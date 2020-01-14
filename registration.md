---
layout: default
title: Registration
description: Register for the AUCTF event here.
---

<style>
.responsive-wrap iframe{ max-width: 100%;}
</style>
<div class="responsive-wrap">
<!-- this is the embed code provided by Google -->
<!--  <iframe src="https://docs.google.com/forms/d/e/1FAIpQLSdcFmMooBJf2HqLN_LzwHIXAADUPNizjLx27EX8QqK77gMqfA/viewform?embedded=true" width="640" height="1880" frameborder="0" marginheight="0" marginwidth="0">Loading…</iframe> -->
<!-- Google embed ends -->
</div>

<!-- Display the countdown timer in an element -->
<h1 id="demo"></h1>

<script>
// Set the date we're counting down to
var countDownDate = new Date("Jan 20, 2020 12:00:00").getTime();

// Update the count down every 1 second
var x = setInterval(function() {

  // Get today's date and time
  var now = new Date().getTime();

  // Find the distance between now and the count down date
  var distance = countDownDate - now;

  // Time calculations for days, hours, minutes and seconds
  var days = Math.floor(distance / (1000 * 60 * 60 * 24));
  var hours = Math.floor((distance % (1000 * 60 * 60 * 24)) / (1000 * 60 * 60));
  var minutes = Math.floor((distance % (1000 * 60 * 60)) / (1000 * 60));
  var seconds = Math.floor((distance % (1000 * 60)) / 1000);

  // Display the result in the element with id="demo"
  document.getElementById("demo").innerHTML = days + " days " + hours + " hours "
  + minutes + " minutes " + seconds + " seconds until the registration is available.";

  // If the count down is finished, write some text
  if (distance < 0) {
    clearInterval(x);
    document.getElementById("demo").innerHTML = "Expired";
  }
}, 1000);
</script>

[back](./)
