<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Romantic Site</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            height: 100vh;
            position: relative;
            background-color: #f0f0f0; /* Light background for contrast */
        }
        .page {
            display: none;
            height: 100vh;
        }
        .page.active {
            display: block;
        }
        .main-text {
            position: absolute;
            top: 50%;
            left: 50%;
            transform: translate(-50%, -50%);
            font-size: 24px;
            text-align: center;
        }
        .arrow {
            display: inline-block;
            font-size: 24px;
            color: black;
            margin-left: 10px;
        }
        .top-right {
            position: absolute;
            top: 10px;
            right: 10px;
            font-size: 12px;
            color: #666;
        }
        .top-left {
            position: absolute;
            top: 10px;
            left: 10px;
            font-size: 12px;
            color: #666;
        }
        .heart-button {
            position: absolute;
            bottom: 10px;
            left: 10px;
            width: 30px;
            height: 30px;
            background-color: transparent;
            border: none;
            cursor: pointer;
            fill: red;
        }
        .heart-svg {
            width: 100%;
            height: 100%;
        }
        .second-page {
            background-color: pink;
            display: flex;
            justify-content: center;
            align-items: center;
            text-align: center;
            padding: 20px;
        }
        .message {
            font-size: 18px;
            line-height: 1.6;
            max-width: 600px;
        }
    </style>
</head>
<body>
    <!-- First Page -->
    <div id="first-page" class="page active">
        <div class="main-text">
            look at the top left of the page
            <span class="arrow">↗️</span>
        </div>
        <div class="top-right">this is the top right stoop</div>
        <div class="top-left">click the small heart on the bottom left of the page</div>
        <button class="heart-button" onclick="showSecondPage()">
            <svg class="heart-svg" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg">
                <path d="M12 21.35l-1.45-1.32C5.4 15.36 2 12.28 2 8.5 2 5.42 4.42 3 7.5 3c1.74 0 3.41.81 4.5 2.09C13.09 3.81 14.76 3 16.5 3 19.58 3 22 5.42 22 8.5c0 3.78-3.4 6.86-8.55 11.54L12 21.35z"/>
            </svg>
        </button>
    </div>

    <!-- Second Page -->
    <div id="second-page" class="page second-page">
        <div class="message">
            Dear Pooper, I cannot be more grateful to the world for giving me the honour of having spent another year with you, as much as it pains me to not be with you either of the times that weve survived a year together i am gonna be selfish and ask you to stick by this weird little man you gave the gift of being your boyfriend so that we can stick together for all the new years to come and hopefully to a year where we can count the next chapters of our life togther side by side hand in hand. I will stop now because as much as i love cheese ik you dont. I love you Moosh Wazir a very happy new year, heres to being together for ALL the years to come.
        </div>
    </div>

    <script>
        function showSecondPage() {
            document.getElementById('first-page').classList.remove('active');
            document.getElementById('second-page').classList.add('active');
        }
    </script>
</body>
</html>
