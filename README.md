<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>TikTok Overlay</title>
    <style>
        body {
            margin: 0;
            overflow: hidden;
            background-color: black;
        }
        .overlay {
            position: absolute;
            width: 100%;
            height: 100%;
        }
        .anonymous-mask {
            position: absolute;
            top: 5%;
            left: 5%;
            width: 100px;
            opacity: 0.7;
            animation: fade 2s infinite alternate;
        }
        @keyframes fade {
            0% { opacity: 0.5; }
            100% { opacity: 1; }
        }
        .chat-box {
            position: absolute;
            bottom: 10%;
            left: 5%;
            width: 300px;
            height: 150px;
            border: 2px solid gold;
            background: rgba(0, 0, 0, 0.6);
            color: gold;
            padding: 10px;
            font-family: Arial, sans-serif;
        }
        .donation-alert {
            position: absolute;
            top: 10%;
            right: 5%;
            width: 250px;
            height: 50px;
            border: 2px solid gold;
            background: rgba(0, 0, 0, 0.7);
            color: gold;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 18px;
            font-family: Arial, sans-serif;
        }
        .username {
            position: absolute;
            bottom: 5%;
            left: 5%;
            color: gold;
            font-size: 24px;
            font-family: Arial, sans-serif;
        }
    </style>
</head>
<body>
    <div class="overlay">
        <img src="https://i.imgur.com/6Yl3hJ5.png" class="anonymous-mask" alt="Anonymous Mask">
        <div class="chat-box">Chat Overlay</div>
        <div class="donation-alert">💰 New Donation!</div>
        <div class="username">@Tajanstveni</div>
    </div>
</body>
</html>
