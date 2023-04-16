<script>
	import Counter from './Counter.svelte';
	import logo from '$lib/images/airisp.png';
</script>

<svelte:head>
	<title>airISP</title>
	<meta name="description" content="airISP" />
</svelte:head>

<section>
	<h1>
		<div class="welcome">
			<picture>
				<img src={logo} alt="" />
			</picture>
		</div>
	</h1>
	<p class="drac-heading drac-heading-lg drac-text-white">Odstávka služieb na:</p>	
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
	}

	@media only screen and (max-width: 450px) {
		h1 {
			font-size: 1.8rem;
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
