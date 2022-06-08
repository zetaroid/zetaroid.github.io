---
title: Gaming
layout: landing
description: 
image: assets/images/gaming.webp
nav-menu: true
---

<!-- Main -->
<div id="main">

<!-- Two -->
<section id="two" class="spotlights">
	<section>
		<a class="image">
			<img src="{% link assets/images/hypetrain.png %}" alt="" data-position="center center" />
		</a>
		<div class="content">
			<div class="inner">
				<header class="major">
					<h3>Current Hype Train: Xenoblade Chronicles 3</h3>
				</header>
				<p>As the follow up to my #1 game of all time, Xenoblade Chronicles 3 holds the current hype train slot!</p>
				<p id="countdown"></p>
			</div>
		</div>
	</section>
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
	<section>
		<a href="best_of_2022.html" class="image">
			<img src="{% link assets/images/bestof2022.png %}" alt="" data-position="25% 25%" />
		</a>
		<div class="content">
			<div class="inner">
				<header class="major">
					<h3>Best of 2022</h3>
				</header>
				<p>What I've played in 2022 and my thoughts on it.</p>
				<ul class="actions">
					<li><a href="best_of_2022.html" class="button">See it!</a></li>
				</ul>
			</div>
		</div>
	</section>
</section>
	
<script>
// Set the date we're counting down to
var countDownDate = new Date("Jul 29, 2022").getTime();

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
  document.getElementById("demo").innerHTML = days + "d " + hours + "h "
  + minutes + "m " + seconds + "s ";
    
  // If the count down is over, write some text 
  if (distance < 0) {
    clearInterval(x);
    document.getElementById("countdown").innerHTML = "RELEASED";
  }
}, 1000);
</script>
	
</div>
