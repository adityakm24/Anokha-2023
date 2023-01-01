<script setup>

</script>

<template>

    <div class="Counter">
       
<section class="counter-section">
<div class="container">
<div class="row">
<div class="col-lg-4">
<div class="counter-text">
<span>Mark your calenders </span>
<h3>Feb 13th, 2023 </h3>
<br /> <span>Register now </span>
</div>
</div>
<div class="col-lg-8">
<div class="cd-timer" id="countdown">
<div class="cd-item">
<span id="days"></span>
<p>Days</p>
</div>
<div class="cd-item">
<span id="hrs"></span>
<p>Hours</p>
</div>
<div class="cd-item">
<span id="mins"></span>
<p>Minutes</p>
</div>
<div class="cd-item">
<span id="secs">32</span>
<p>Seconds</p>
</div>
</div>
</div>
</div>
</div>
</section>
    </div>

</template>


<script scoped>
// Set the date we're counting down to
var countDownDate = new Date("Feb 5, 2023 15:37:25").getTime();

// Update the count down every 1 second
var x = setInterval(function () {

    var now = new Date().getTime();

    var distance = countDownDate - now;

    var days = Math.floor(distance / (1000 * 60 * 60 * 24));
    var hours = Math.floor((distance % (1000 * 60 * 60 * 24)) / (1000 * 60 * 60));
    var minutes = Math.floor((distance % (1000 * 60 * 60)) / (1000 * 60));
    var seconds = Math.floor((distance % (1000 * 60)) / 1000);
    document.getElementById("days").innerHTML = days;
    document.getElementById("hrs").innerHTML  = hours;
    document.getElementById("mins").innerHTML  = minutes;
    document.getElementById("secs").innerHTML  = seconds;

    if (distance < 0) {
        clearInterval(x);
        document.getElementById("days").innerHTML = 0;
    document.getElementById("hrs").innerHTML  = 0;
    document.getElementById("mins").innerHTML  = 0;
    document.getElementById("secs").innerHTML  = 0;
    }
}, 1000);
</script>

<style scoped>
.Counter {
    background-color: #4158D0;
    background-image: linear-gradient(295deg, #4158D0 0%, #C850C0 46%, #FFCC70 100%);
    padding: 30px;
    margin: auto;
    text-align: center;
    color: white;
}


.counter-section {
	padding: 40px 0;
}

.counter-section .counter-text span {
	font-size: 16px;
	color: #ffffff;
}

.counter-section .counter-text h3 {
	color: #ffffff;
	font-weight: 700;
	line-height: 38px;
	margin-top: 10px;
}

.counter-section .cd-timer {
	text-align: right;
}

.counter-section .cd-timer .cd-item {
	display: inline-block;
	text-align: center;
	margin-left: 35px;
	height: 120px;
	width: 120px;
	padding-top: 32px;
	position: relative;
}

.counter-section .cd-timer .cd-item:after {
	position: absolute;
	left: 0;
	top: 0;
	width: 100%;
	height: 100%;
	border: 2px solid #ffffff;
	content: "";
	opacity: 0.1;
	border-radius: 4px;
}

.counter-section .cd-timer .cd-item:first-child {
	margin-left: 0;
}

.counter-section .cd-timer .cd-item span {
	font-size: 60px;
	color: #ffffff;
	font-weight: 600;
	line-height: 30px;
}

.counter-section .cd-timer .cd-item p {
	font-size: 18px;
	color: #ffffff;
	margin-bottom: 0;
	line-height: 30px;
}

@media only screen and (min-width: 992px) and (max-width: 1199px) {

	.counter-section .cd-timer .cd-item {
		margin-left: 25px;
	}
}

@media only screen and (max-width: 991px) {
    .counter-section .counter-text {
		margin-bottom: 30px;
	}
	.counter-section .cd-timer {
		text-align: left;
	}
}

@media only screen and (max-width: 767px) {
	.counter-section .cd-timer .cd-item {
		margin-bottom: 10px;
	}
}
.counter-section .cd-timer .cd-item {
		margin-right: 10px;
		margin-left: 0;
	}
	.counter-section .cd-timer .cd-item:last-child {
		margin-right: 0;
	}

    @media only screen and (max-width: 479px) {
	.counter-section .cd-timer .cd-item {
		margin-right: 10px;
		margin-left: 0;
	}
}
</style>
