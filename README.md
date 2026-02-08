# naman-sharma64
this is my 21th repository
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Snapchat Spotlight UI</title>
    <style>
        :root {
            --snap-yellow: #FFFC00;
            --snap-shadow: rgba(0, 0, 0, 0.3);
        }

        body {
            font-family: 'Avenir Next', 'Helvetica Neue', Helvetica, sans-serif;
            background-color: #1a1a1a;
            margin: 0;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            overflow: hidden;
        }

        /* Phone Container */
        .snap-container {
            width: 375px;
            height: 667px;
            background-color: #000;
            border-radius: 40px;
            position: relative;
            overflow: hidden;
            box-shadow: 0 20px 40px rgba(0,0,0,0.5);
            border: 8px solid #333;
        }

        /* Fullscreen Video Background */
        .video-bg {
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
        }

        .video-bg iframe {
            width: 100%;
            height: 100%;
            border: none;
            transform: scale(1.8); /* Zoom to fill vertical screen */
        }

        /* Top Icons */
        .top-nav {
            position: absolute;
            top: 30px;
            left: 0;
            width: 100%;
            padding: 0 20px;
            display: flex;
            justify-content: space-between;
            box-sizing: border-box;
            z-index: 10;
        }

        .icon-circle {
            width: 40px;
            height: 40px;
            background: rgba(0,0,0,0.4);
            border-radius: 50%;
            display: flex;
            justify-content: center;
            align-items: center;
            color: white;
            font-size: 20px;
        }

        /* Right Side Actions */
        .side-actions {
            position: absolute;
            right: 15px;
            bottom: 120px;
            display: flex;
            flex-direction: column;
            gap: 20px;
            z-index: 10;
        }

        .action-item {
            text-align: center;
            color: white;
            font-size: 12px;
            text-shadow: 1px 1px 3px var(--snap-shadow);
        }

        .action-icon {
            font-size: 28px;
            margin-bottom: 4px;
        }

        /* Bottom Info & Input */
        .bottom-ui {
            position: absolute;
            bottom: 0;
            width: 100%;
            padding: 20px;
            background: linear-gradient(transparent, rgba(0,0,0,0.8));
            box-sizing: border-box;
            color: white;
        }

        .username { font-weight: bold; margin-bottom: 5px; font-size: 16px; }
        .caption { font-size: 14px; margin-bottom: 15px; }

        .chat-bar {
            background: rgba(255, 255, 255, 0.2);
            backdrop-filter: blur(10px);
            border-radius: 25px;
            padding: 10px 20px;
            font-size: 14px;
            display: flex;
            justify-content: space-between;
        }
    </style>
</head>
<body>

    <div class="snap-container">
        <div class="video-bg">
            <iframe src="https://www.youtube.com/embed/dQw4w9WgXcQ?controls=0&autoplay=1&mute=1&loop=1&playlist=dQw4w9WgXcQ" allow="autoplay"></iframe>
        </div>

        <div class="top-nav">
            <div class="icon-circle">👤</div>
            <div class="icon-circle">🔍</div>
        </div>

        <div class="side-actions">
            <div class="action-item"><div class="action-icon">❤️</div>24k</div>
            <div class="action-item"><div class="action-icon">💬</div>156</div>
            <div class="action-item"><div class="action-icon">↪️</div>Share</div>
        </div>

        <div class="bottom-ui">
            <div class="username">the_coding_engineer ✨</div>
            <div class="caption">Building UIs from Dadri to Bangalore! 🚀 #BTech #SSBPrep</div>
            <div class="chat-bar">
                <span>Send a Chat</span>
                <span>📷</span>
            </div>
        </div>
    </div>

</body>
</html>
