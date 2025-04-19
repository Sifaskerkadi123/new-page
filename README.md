<!DOCTYPE html>
<html lang="en">

<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>My Interactive Web Page</title>
  <link rel="stylesheet" href="css.css"
  <style>
    body {
      font-family: Arial, sans-serif;
      background-color: #f0f4f8;
      margin: 0;
      padding: 20px;
      transition: background-color 0.5s;
      /* Smooth transition */
    }

    .container {
      max-width: 800px;
      margin: auto;
      background: white;
      border-radius: 8px;
      box-shadow: 0 2px 10px rgba(0, 0, 0, 0.1);
      padding: 20px;
    }

    h1 {
      color: #333;
      text-align: center;
      font-size: 2.5em;
      margin-bottom: 0.5em;
    }

    p {
      color: #555;
      line-height: 1.6;
      font-size: 1.2em;
      text-align: justify;
      margin-bottom: 20px;
    }

    .button {
      display: inline-block;
      background-color: #007BFF;
      color: white;
      padding: 10px 15px;
      border-radius: 5px;
      text-decoration: none;
      text-align: center;
      transition: background-color 0.3s ease;
      margin: 5px;
      /* Add margin for spacing */
    }

    .button:hover {
      background-color: #0056b3;
    }

    footer {
      text-align: center;
      margin-top: 20px;
      font-size: 0.9em;
      color: #777;
    }
  </style>
</head>

<body>
  <div class="container">
    <h1>Welcome to My Web Page!</h1>
    <p id="myParagraph">Hi! I am Sifas and I am from Algeria and this is my web page, click the buttoms for a gift</p>
    <a href="#" class="button" id="alertButton">Click Me!</a>
    <a href="#" class="button" id="changeColorButton">Change Background Color</a>
    <a href="#" class="button" id="toggleTextButton">Toggle Text</a>
  </div>
  <footer>
    <p>Created with ❤️ using HTML & CSS</p>
  </footer>
  <script>
    // Alert on Click
    document.getElementById('alertButton').addEventListener('click', function(event) {
      event.preventDefault(); // Prevent default link behavior
      alert('Yeddek fezzebi');
    });
    // Change Background Color
    document.getElementById('changeColorButton').addEventListener('click', function(event) {
      event.preventDefault();
      document.body.style.backgroundColor =
        document.body.style.backgroundColor === 'lightblue' ? '#f0f4f8' : 'lightblue';
    });
    // Toggle Text
    document.getElementById('toggleTextButton').addEventListener('click', function(event) {
      event.preventDefault();
      const paragraph = document.getElementById('myParagraph');
      if (paragraph.innerHTML === 'This is a simple web page created using HTML and CSS. It has been styled to be more visually appealing.') {
        paragraph.innerHTML = 'You toggled the text!';
      } else {
        paragraph.innerHTML = 'This is a simple web page created using HTML and CSS. It has been styled to be more visually appealing.';
      }
    });
  </script>
</body>

</html>
