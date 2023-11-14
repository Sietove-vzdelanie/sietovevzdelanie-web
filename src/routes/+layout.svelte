<script>
	import Header from './Header.svelte';
	import './styles.css';

	let teraz = new Date(), month, day, year;
	year = teraz.getFullYear();

</script>

<div class="app">
	<Header />

	<main>
		<slot />
	</main>

	<footer>
		<p class="drac-text drac-text-white"><center>podpora@sietovevzdelanie.eu</center><br>{year} Sieťové vzdelanie <a href="/podmienky">podmienky služby</a></p>
	</footer>
</div>

<style>
	a { text-decoration: none; }
	a:link { text-decoration: none; }
	a:visited { text-decoration: none; }
	a:hover { text-decoration: none; }
	a:active { text-decoration: none; }
	.app {
		display: flex;
		flex-direction: column;
		min-height: 100vh;
	}

	main {
		flex: 1;
		display: flex;
		flex-direction: column;
		padding: 1rem;
		width: 100%;
		max-width: 64rem;
		margin: 0 auto;
		box-sizing: border-box;
	}

	footer {
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;
		padding: 12px;
	}

	footer a {
		font-weight: bold;
	}

	a { text-decoration: none; }

	@media (min-width: 480px) {
		footer {
			padding: 12px 0;
		}
	}
</style>
