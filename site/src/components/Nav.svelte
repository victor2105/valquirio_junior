<script>
	export let segment;

	let y = 0;

	let open = false;

</script>

<svelte:window bind:scrollY={y}/>

<!-- Navigation-->
<nav class="navbar navbar-expand-lg navbar-light fixed-top {y > 100 ? 'navbar-shrink' : '' } " id="mainNav">
	<div class="container">
		<a class="navbar-brand js-scroll-trigger" on:click={() => open = false} href="#page-top">Start Bootstrap</a>
		<button class="navbar-toggler navbar-toggler-right" type="button" on:click={() => open = !open} aria-expanded={open}>
			Menu
			<i class="fas fa-bars"></i>
		</button>
		<div class="collapse navbar-collapse {open ? 'show' : ''}" id="navbarResponsive">
			<ul class="navbar-nav ml-auto">
				<li class="nav-item"><a class="nav-link js-scroll-trigger" on:click={() => open = false} href="#about">About</a></li>
				<li class="nav-item"><a class="nav-link js-scroll-trigger" on:click={() => open = false} href="#projects">Projects</a></li>
				<li class="nav-item"><a class="nav-link js-scroll-trigger" on:click={() => open = false} href="#signup">Contact</a></li>
			</ul>
		</div>
	</div>
</nav>