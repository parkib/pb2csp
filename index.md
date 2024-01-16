---
layout: home
search_exclude: true
---
My trimester 2 repository --> to document notes/progress/ideation/review tickets/etc. 



# recent posts

<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <style>
    body {
      margin: 0;
      overflow: hidden;
    }

    #loading-overlay {
      position: fixed;
      top: 0;
      left: 0;
      width: 100%;
      height: 100%;
      background: #191f26;
      color: #fff;
      display: flex;
      justify-content: center;
      align-items: center;
      z-index: 9999;
      animation: fadeInAndOut 8s forwards;
    }

    #loading-gif {
      max-width: 100%;
      max-height: 100%;
    }

    #new-screen {
      display: none;
      position: fixed;
      top: 0;
      left: 0;
      width: 100%;
      height: 100%;
      background: #ffdb98;
      z-index: 9999;
      animation: fadeInAndOutNewScreen 5s forwards;
    }

    #panda-gif {
      position: fixed;
      bottom: 0;
      left: 50%;
      transform: translateX(-50%);
      max-width: 100%;
      max-height: 50vh;
    }

    @keyframes fadeInAndOut {
      0% {
        opacity: 1;
      }
      25% {
        opacity: 1;
      }
      100% {
        opacity: 0;
        display: none;
      }
    }

    @keyframes fadeInAndOutNewScreen {
      0% {
        opacity: 0;
      }
      100% {
        opacity: 1;
      }
    }

    @keyframes fadeOutNewScreen {
      0% {
        opacity: 1;
      }
      100% {
        opacity: 0;
        display: none;
      }
    }
  </style>
</head>
<body>
  <div id="loading-overlay">
    <img id="loading-gif" src="load.gif" alt="Loading GIF">
  </div>

  <div id="new-screen">
    <img id="panda-gif" src="creepy.gif" alt="Panda GIF">
  </div>

  <!-- Your actual webpage content goes here -->

  <script>
    // Simulate a delay (e.g., loading resources) before hiding the loading overlay
    setTimeout(function() {
      var loadingOverlay = document.getElementById('loading-overlay');
      loadingOverlay.style.display = 'none';

      var newScreen = document.getElementById('new-screen');
      newScreen.style.display = 'block';

      // After 2 seconds, fade out the new screen
      setTimeout(function() {
        newScreen.style.animation = 'fadeOutNewScreen 3s forwards';
      }, 3000);

    }, 8000); // Simulating an 8-second loading time

    // You can add more JavaScript code here if needed
  </script>
</body>
</html>
