<!DOCTYPE html>
<html lang="en">

<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Hidden Message Website</title>
  <style>
    body {
      display: flex;
      justify-content: center;
      align-items: center;
      height: 100vh;
      margin: 0;
      background-color: #f0f0f0;
    }

    .container {
      text-align: center;
      position: relative;
    }

    button {
      position: fixed; /* Use 'fixed' or 'relative' as per your preference */
      left: 50px; /* Adjust left position here */
      top: 50px; /* Adjust top position here */
      padding: 10px 20px;
      font-size: 16px;
      background-color: #9C72D3;
      color: #fff;
      border: none;
      cursor: pointer;
      border-radius: 5px;
    }

    button span {
      display: inline-block;
    }

    button:hover {
      background-color: #936BC6;
    }

    #hiddenMessage {
      display: none;
      margin-top: 20px;
      padding: 10px;
      background-color: #333;
      color: #fff;
      border-radius: 5px;
    }
  </style>
</head>

<body>
  <div class="container">
    <button id="revealButton"><span>Dark Mode</span></button>
    <div id="hiddenMessage" class="hidden">
      Congratulations! You found the hidden message!
    </div>
    </div>

    <br>

    <!-- Adding a text input box -->
    <label for="nameInput">Enter your name:</label>
    <input type="text" id="nameInput" placeholder="Your name...">
  </div>

  <script>
    const button = document.getElementById('revealButton');
    const hiddenMessage = document.getElementById('hiddenMessage');

    button.addEventListener('click', () => {
      document.body.style.backgroundColor = '#303030';
      hiddenMessage.style.display = 'block';
    });
  </script>
</body>

</html>
