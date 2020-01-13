---
layout: default
---

<p id="demo"></p>

<script>
var countDownDate = new Date("Feb 29, 2021 9:00:00").getTime();
var x = setInterval(function() {
  var now = new Date().getTime();
  var distance = countDownDate - now;
  var days = Math.floor(distance / (1000 * 60 * 60 * 24));
  var hours = Math.floor((distance % (1000 * 60 * 60 * 24)) / (1000 * 60 * 60));
  var minutes = Math.floor((distance % (1000 * 60 * 60)) / (1000 * 60));
  var seconds = Math.floor((distance % (1000 * 60)) / 1000);
  document.getElementById("demo").innerHTML = days + " days " + hours + " hours " + minutes + "  minutes " + seconds + " seconds until AUCTF.";
  if (distance < 0) {
    clearInterval(x);
    document.getElementById("demo").innerHTML = "Expired";
  }
}, 1000);
</script>
