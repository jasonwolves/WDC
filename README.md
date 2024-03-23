<!DOCTYPE html>
<html>
<head>
<style>
.container { 
  height: 200px;
  position: relative;
  border: 3px solid green; 
}

.center {
  margin: 0;
  position: absolute;
  top: 50%;
  left: 50%;
  -ms-transform: translate(-50%, -50%);
  transform: translate(-50%, -50%);
}
</style>
</head>
<body>

 <div class="container">
  <div class="center">
    <p></p>
    <p>Deaths In The World</p>
    <button onclick="startCounting()">Start</button>
    <script>
        let count = 0;
        let intervalId; // to store the interval ID
        function startCounting() {
            // Check if the counting is already in progress
            if (!intervalId) {
                intervalId = setInterval(function() {
                    count++;
                    document.getElementById('countDisplay').innerText = "" + count;
                }, 1500); // 1500 milliseconds = 1.5 seconds
            }
        }
    </script>
 <br>
 <br>
    <div id="countDisplay"></div>
    </div>
</div>

</body>
</html>


