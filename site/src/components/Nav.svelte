<script>
	export let segment;

	let y = 0;

</script>

<svelte:window bind:scrollY={y}/>

<!-- Navigation-->
<nav class="navbar navbar-expand-lg navbar-light fixed-top {y > 100 ? 'navbar-shrink' : '' } " id="mainNav">
	<div class="container">
		<a class="navbar-brand js-scroll-trigger" href="#page-top">Start Bootstrap</a>
		<button class="navbar-toggler navbar-toggler-right" type="button" data-toggle="collapse" data-target="#navbarResponsive" aria-controls="navbarResponsive" aria-expanded="false" aria-label="Toggle navigation">
			Menu
			<i class="fas fa-bars"></i>
		</button>
		<div class="collapse navbar-collapse" id="navbarResponsive">
			<ul class="navbar-nav ml-auto">
				<li class="nav-item"><a class="nav-link js-scroll-trigger" href="#about">About</a></li>
				<li class="nav-item"><a class="nav-link js-scroll-trigger" href="#projects">Projects</a></li>
				<li class="nav-item"><a class="nav-link js-scroll-trigger" href="#signup">Contact</a></li>
			</ul>
		</div>
	</div>
</nav>