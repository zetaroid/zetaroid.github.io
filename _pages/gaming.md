---
title: Gaming
layout: landing
description: 
image: assets/images/gaming.webp
nav-menu: true
order: 5
permalink: "gaming"
---

<!-- Main -->
<div id="main">

<!-- Two -->
<section id="two" class="spotlights">
	<section>
		<a href="top_games.html" class="image">
			<img src="{% link assets/images/smash.png %}" alt="" data-position="center center" />
		</a>
		<div class="content">
			<div class="inner">
				<header class="major">
					<h3>Top 10 Games of All Time</h3>
				</header>
				<p>A completely biased and not at all objective list of my top 10 games of all time.</p>
				<ul class="actions">
					<li><a href="top_games.html" class="button">See it!</a></li>
				</ul>
			</div>
		</div>
	</section>
</section>
	
<script>
// Set the date we're counting down to
var countDownDate = new Date("Nov 18, 2022").getTime();

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
    
  // Output the result in an element with id="demo"
  document.getElementById("countdown").innerHTML = "Countdown to release: " + days + "d " + hours + "h "
  + minutes + "m " + seconds + "s ";
    
  // If the count down is over, write some text 
  if (distance < 0) {
    clearInterval(x);
    document.getElementById("countdown").innerHTML = "RELEASED";
  }
}, 1000);
</script>
	
</div>
