<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Special Proposal for Vishu</title>
    <style>
        body { 
            font-family: Arial, sans-serif; 
            text-align: center; 
            background-color: #f7f3f1; 
            margin: 0; 
            padding: 0;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            flex-direction: column;
        }
        .container {
            display: none;
        }
        h1 { color: #9c2e3c; font-size: 2.5em; }
        p { font-size: 1.5em; margin-bottom: 20px; color: #333; }
        button { 
            padding: 15px 30px; 
            background-color: #9c2e3c; 
            color: white; 
            border: none; 
            cursor: pointer; 
            font-size: 1.2em; 
            margin-top: 20px; 
            border-radius: 5px;
        }
        button:hover { 
            background-color: #7a1e2a; 
        }
        .hidden {
            display: none;
        }
    </style>
</head>
<body>

    <!-- Welcome Message -->
    <div id="page1" class="container" style="display:block;">
        <h1>Hey Vishu, I have something special for you...</h1>
        <p>I want to tell you something that comes straight from my heart. Are you ready for this surprise?</p>
        <button onclick="showNext('page2')">Next</button>
    </div>

    <!-- Second Page -->
    <div id="page2" class="container">
        <h1>Our journey started in the most beautiful way...</h1>
        <p>Every moment spent with you feels like a beautiful dream. You changed my world completely.</p>
        <button onclick="showNext('page3')">Next</button>
    </div>

    <!-- Third Page -->
    <div id="page3" class="container">
        <h1>Your smile is my light...</h1>
        <p>Every day with you is a new adventure. You bring joy to my life, and I cherish every moment with you.</p>
        <button onclick="showNext('page4')">Next</button>
    </div>

    <!-- Fourth Page -->
    <div id="page4" class="container">
        <h1>You are my world...</h1>
        <p>I can't imagine a future without you. You are the most precious part of my life, and I want to spend forever with you.</p>
        <button onclick="showNext('page5')">Next</button>
    </div>

    <!-- Fifth Page -->
    <div id="page5" class="container">
        <h1>Will you be mine forever?</h1>
        <p>Vishu, I want to walk this journey of life with you. Will you be my partner, my love, forever?</p>
        <button onclick="showNext('page6')">Yes, forever</button>
    </div>

    <!-- Sixth Page (Celebration) -->
    <div id="page6" class="container">
        <h1>Our journey begins...</h1>
        <p>You said yes, and my heart is full of joy! Together, we will write the most beautiful chapters of our lives.</p>
        <button onclick="showNext('page7')">Continue this journey</button>
    </div>

    <!-- Seventh Page (Conclusion) -->
    <div id="page7" class="container">
        <h1>Our love story begins now...</h1>
        <p>With you by my side, I know we can conquer anything. Let's make our dreams come true, together.</p>
        <button onclick="window.location.href='https://www.example.com'">Start our journey</button>
    </div>

    <script>
        function showNext(pageId) {
            // Hide all pages
            var pages = document.querySelectorAll('.container');
            pages.forEach(function(page) {
                page.style.display = 'none';
            });
            // Show the next page
            document.getElementById(pageId).style.display = 'block';
        }
    </script>

</body>
</html>
