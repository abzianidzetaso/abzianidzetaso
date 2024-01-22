<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Special Message for You</title>
  <style>
    body {
      background-color: #fff; /* White background */
      text-align: center;
      font-family: Arial, sans-serif;
    }
    img {
      max-width: 100%;
      height: auto;
    }
  </style>
</head>
<body>

  <h1>Hi there, my love!</h1>
  
  <p>Click the link below to reveal a special message:</p>
  
  <a href="#" onclick="showMessage()">
    Click me to see a bunny with flowers!
  </a>

  <div id="message" style="display: none;">
    <img src="bunny_with_flowers.jpg" alt="Bunny with Flowers">
    <p>Will you go out with me?</p>
    <button onclick="decision('yes')">Yes</button>
    <button onclick="decision('no')">No</button>
  </div>

  <script>
    function showMessage() {
      document.getElementById('message').style.display = 'block';
    }

    function decision(answer) {
      if (answer === 'yes') {
        alert('Bunny is happy! 🐰💖');
      } else {
        alert('Bunny is sad. 😢 Try again another time.');
        // You can customize this part to add more actions if needed.
      }
    }
  </script>

</body>
</html>
