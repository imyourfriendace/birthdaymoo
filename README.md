
<html>
  <head>
    <title>^^</title>
    <style>
      body {
        background: url('https://cdn.wallpapersafari.com/97/23/5c8bhS.jpg') no-repeat center center fixed; /* Set the background image */
        background-size: cover; /* Scale the image to cover the entire background */
        font-family: Algerian, sans-serif;
        text-align: center;
      }
      
      h1 {
        margin-top: 50px;
      }
      
      #countdown {
        font-size: 48px;
        margin-top: 20px;
        color: #333;
      }
      
      #youtube-link {
        margin-top: 20px;
      }
      
      #youtube-link a {
        color: #fff;
        text-decoration: none;
        border: 2px solid #fff;
        padding: 10px 20px;
        border-radius: 5px;
        transition: background-color 0.3s ease;
      }
      
      #youtube-link a:hover {
        background-color: #fff;
        color: #333;
      }
    </style>
  </head>
  <body>
    <h1>LAST BIRTHDAY</h1>
    <div id="countdown"></div>
    
    <div id="youtube-link">
      <a href="https://youtu.be/tL6SQ2PGXV4/" target="_blank">HULAT</a>
    </div>
    
    <script>
      // Set the date we're counting down to
      var countDownDate = new Date("Jul 23, 2023 00:00:00").getTime();

      // Update the countdown every 1 second
      var x = setInterval(function() {

        // Get the current date and time
        var now = new Date().getTime();

        // Find the distance between now and the countdown date
        var distance = countDownDate - now;

        // Calculate days, hours, minutes, and seconds left
        var days = Math.floor(distance / (1000 * 60 * 60 * 24));
        var hours = Math.floor((distance % (1000 * 60 * 60 * 24)) / (1000 * 60 * 60));
        var minutes = Math.floor((distance % (1000 * 60 * 60)) / (1000 * 60));
        var seconds = Math.floor((distance % (1000 * 60)) / 1000);

        // Display the countdown in the #countdown div
        document.getElementById("countdown").innerHTML = days + "d " + hours + "h "
        + minutes + "m " + seconds + "s ";

        // If the countdown is over, display a message and show the YouTube link
        if (distance < 0) {
          clearInterval(x);
          document.getElementById("countdown").innerHTML = "EXPIRED";
          document.getElementById("youtube-link").style.display = "block";
        }
      }, 1000);
    </script>
  </body>
</html>
