# heykiddositsmomma
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Personal Profile & Blog</title>
    <style>
        body {
            font-family: 'Arial', sans-serif;
            background-color: #f0f8ff; /* Light coastal blue */
            color: #333;
            margin: 0;
            padding: 0;
        }
        header {
            background: url('https://www.example.com/coastal-background.jpg') no-repeat center center/cover;
            color: white;
            padding: 20px;
            text-align: center;
        }
        .container {
            max-width: 800px;
            margin: auto;
            padding: 20px;
        }
        h1, h2 {
            color: #004d00; /* Deep green for coastal feel */
        }
        .section {
            margin-bottom: 30px;
        }
        .video {
            margin-top: 10px;
        }
        .code-container {
            display: none;
            text-align: center;
            margin: 20px 0;
        }
        .code-container input {
            padding: 10px;
            font-size: 16px;
        }
        .code-container button {
            padding: 10px 20px;
            font-size: 16px;
            background-color: #004d00;
            color: white;
            border: none;
            cursor: pointer;
        }
        .code-container button:hover {
            background-color: #003300;
        }
        footer {
            text-align: center;
            padding: 10px;
            background-color: #004d00;
            color: white;
        }
    </style>
</head>
<body>
    <header>
        <h1>Welcome to My Personal Profile</h1>
    </header>
    <div class="container">
        <!-- Code unlock section -->
        <div class="code-container" id="code-container">
            <h2>Enter the Code to Unlock Content</h2>
            <input type="text" id="code-input" placeholder="Enter code here">
            <button onclick="unlockContent()">Submit</button>
        </div>

        <!-- About Me section -->
        <div class="section" id="about-me">
            <h2>About Me</h2>
            <p>Hello! I'm [Your Name], a coastal enthusiast with a passion for [Your Interests]. Welcome to my personal profile and blog where I share my adventures, insights, and dreams.</p>
        </div>

        <!-- Videos section -->
        <div class="section" id="videos">
            <h2>Videos</h2>
            <div class="video">
                <p>Video 1</p>
                <iframe width="560" height="315" src="https://www.youtube.com/embed/[VIDEO_ID]" frameborder="0" allowfullscreen></iframe>
            </div>
            <!-- Add more videos as needed -->
        </div>

        <!-- Q&A section -->
        <div class="section" id="qa">
            <h2>Q&A</h2>
            <p>Q: What inspires you?</p>
            <p>A: I find inspiration in nature, especially the coastal landscapes. They remind me of the beauty and serenity of life.</p>
            <!-- Add more Q&A as needed -->
        </div>

        <!-- 5-Year Plan section -->
        <div class="section" id="five-year-plan">
            <h2>5-Year Plan</h2>
            <p>In the next five years, I aim to:</p>
            <ul>
                <li>Travel to new coastal destinations</li>
                <li>Expand my knowledge and skills in [Your Field]</li>
                <li>Build a community around my passions</li>
                <!-- Add more goals as needed -->
            </ul>
        </div>
    </div>
    <footer>
        <p>© 2024 [Your Name]. All rights reserved.</p>
    </footer>

    <script>
        // Unlock content functionality
        function unlockContent() {
            const codeInput = document.getElementById('code-input').value;
            const correctCode = 'YOUR_CODE_HERE'; // Replace with your code

            if (codeInput === correctCode) {
                document.getElementById('code-container').style.display = 'none';
                document.getElementById('about-me').style.display = 'block';
                document.getElementById('videos').style.display = 'block';
                document.getElementById('qa').style.display = 'block';
                document.getElementById('five-year-plan').style.display = 'block';
            } else {
