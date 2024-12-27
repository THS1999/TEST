<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Click Heart to Reveal Text</title>
    <style>
        body {
            font-family: 'Times New Roman', sans-serif;
            text-align: center;
            margin-top: 50px;
        }
        
        .heart {
            font-size: 100px;
            cursor: pointer;
            transition: transform 0.2s;
        }

        .heart:hover {
            transform: scale(1.2);
        }

        .hidden-text {
            display: none;
            margin-top: 20px;
            font-size: 20px;
            color: #555;
        }
    </style>
</head>
<body>

    <!-- Cartoon Red Heart -->
    <div class="heart" id="heart">❤️</div>

    <!-- Hidden Text -->
    <div class="hidden-text" id="text">Dear Daisy, I love u <3 </div>

    <script>
        // Get the heart and text elements
        const heart = document.getElementById('heart');
        const text = document.getElementById('text');
        
        // Add an event listener to the heart element
        heart.addEventListener('click', function() {
            // Toggle the visibility of the text
            text.style.display = text.style.display === 'none' ? 'block' : 'none';
        });
    </script>

</body>
</html>
