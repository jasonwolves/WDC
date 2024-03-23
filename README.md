<html>
<head>
<link rel="stylesheet" type="text/css" href="README.md">
    <title>Login page</title>
<style>
h2 {text-align: center;}
     <style>
    body {
.container { 
  height: 200px;
  position: relative;
  border: 3px solid black; 
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
<body>
<h2><iframe title='Number of deaths' src='https://www.theworldcounts.com/embeds/counters/126?background_color=white&color=black&font_family=%22Helvetica+Neue%22%2C+Arial%2C+sans-serif&font_size=14' style='border: none' height='140' width='500'></iframe></h2>
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
