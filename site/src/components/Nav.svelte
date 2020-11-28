<script>
	let y = 0;
	let open = false;

</script>

<style>	
.logo-font {
    font-family: 'Satisfy', cursive;
}
</style>

<svelte:window bind:scrollY={y}/>

<!-- Navigation-->
<nav class="navbar navbar-expand-lg navbar-light fixed-top {y > 100 ? 'navbar-shrink' : '' } " id="mainNav">
	<div class="container">

		<a class="navbar-brand logo-font text-gradient " on:click={() => open = false} href="#page-top">Kirro Mass</a>

		<button class="navbar-toggler navbar-toggler-right" type="button" on:click={() => open = !open} aria-expanded={open}>
			Menu
			<i class="fas fa-bars"></i>
		</button>
		<div class="collapse navbar-collapse {open ? 'show' : ''}" id="navbarResponsive">
			<ul class="navbar-nav ml-auto">
				<li class="nav-item"><a class="nav-link js-scroll-trigger" on:click={() => open = false} href="#about">Sobre</a></li>
				<li class="nav-item"><a class="nav-link js-scroll-trigger" on:click={() => open = false} href="#projects">Comentários</a></li>
				<li class="nav-item"><a class="nav-link js-scroll-trigger" on:click={() => open = false} href="#signup">Contatos</a></li>
			</ul>
		</div>
	</div>
</nav>