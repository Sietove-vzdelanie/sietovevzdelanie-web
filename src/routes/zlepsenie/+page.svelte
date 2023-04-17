<script>
	import { page } from '$app/stores';
	import github from '$lib/images/github.svg';

	async function redirect() {
		window.location.assign("/");
	}
</script>

<svelte:head>
	<title>Návrh na zlepšenie</title>
	<meta name="description" content="Návrh na zlepšenie" />
</svelte:head>



<div class="text-column">
	<div class="drac-box drac-card drac-card-subtle drac-border-purple drac-p-md drac-m-md">
    <span class="drac-text drac-line-height drac-text-white">
	Návrhy na zlepšenie obsahu, prípadne chyby alebo dizajnové zmeny posielajte na <i>podpora@sietovevzdelanie.eu</i>	
	</span>
 </div>
 <center><button aria-current={$page.url.pathname === '/' ? 'page' : undefined} on:click={redirect} style="margin-top: 1em; margin-left:1em; width:6em" class="drac-btn drac-bg-purple drac-m-sm drac-btn-lg">
	SPÄŤ</button></center>
</div>

