<script>
	import Counter from './Counter.svelte';
	import logo from '$lib/images/airisp.png';
	import { redirect } from '@sveltejs/kit';

	async function redirectt() {
		window.location.assign("https://obsah.sietovevzdelanie.eu/course/view.php?id=3");
	}
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
		<h1 class="drac-text drac-text-purple-cyan">Sieťové <br> Vzdelanie</h1>	
	</div>

	<br><br>

	<button on:click={redirectt} class="drac-btn drac-bg-purple-cyan drac-m-sm">Ukážka kurzov</button>

	<br><br><br><br><br><br>

	<p class="drac-heading drac-heading-lg drac-text-white">Obsah sa spúšťa za:</p>	
	<Counter />
</section>

<style>
	section {
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;
		flex: 0.6;
	}

	h1 {
		width: 100%;
		font-size: 4rem;
	}

	@media only screen and (max-width: 450px) {
		h1 {
			font-size: 3rem;
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
</style>
