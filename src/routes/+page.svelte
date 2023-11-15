<script>
	import Counter from './Counter.svelte';
</script>

<svelte:head>
	<title>Sieťové vzdelanie</title>
	<meta name="description" content="Sieťové vzdelanie" />
</svelte:head>

<section>
	
	<div class="welcome">
		<!-- <picture>
			<img src={logo} alt="" />
		</picture> -->
		<h1 class="drac-text drac-text-purple-cyan">Sieťové<br>Vzdelanie</h1>	
	</div>

	<div style="height: 2em"></div>
	
	<a href="https://obsah.sietovevzdelanie.eu/" class="drac-btn drac-bg-purple-cyan drac-m-sm drac-btn-lg">Ukážka kurzov</a>

	<div style="height: 6em"></div>
	
	<p class="drac-heading drac-heading-lg drac-text-white">Nový obsah dostupný za:</p>	
	<Counter />
</section>

<style>
	section {
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;
		flex: 0.2;
	}

	h1 {
		width: 100%;
		font-size: 4rem;
	}

	@media only screen and (max-width: 450px) {
		h1 {
			font-size: 3.5rem;
		}
	}

	.welcome {
		display: block;
		position: relative;
		padding: 0 0 0 0;
		align-items: center;
	}

	.welcome img {
		height: 8em;
		margin: auto;
		display: block;
		pointer-events: none;
	
	}
	a { 
		text-decoration: none;
		color: black;
	}
	a:link { text-decoration: none; }
	a:visited { text-decoration: none; }
	a:hover { text-decoration: none; }
	a:active { text-decoration: none; }
</style>
