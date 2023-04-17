<script>
	import { page } from '$app/stores';
	import github from '$lib/images/github.svg';

	async function redirect() {
		window.location.assign("/");
	}
</script>

<svelte:head>
	<title>Podmienky služby</title>
	<meta name="description" content="Podmienky" />
</svelte:head>



<div class="text-column">
	<div class="drac-box drac-card drac-card-subtle drac-border-purple drac-p-md drac-m-md">
    <span class="drac-text drac-line-height drac-text-white">
		<b>Všetok náš obsah je voľne šíritelný a dostupný pre každého bez akýchkoľvek poplatkov. Obsah nebude nikdy spoplatnený a slúži len na informačné účely.</b>
<br><br><b>Zdrojový kód:<br><br></b>
Zdrojový kód tejto webovej stránky spolu s celým obsahom je voľne dostupný na githube (odkaz v pravom hornom rohu) pod licenciou GNU GENERAL PUBLIC LICENSE Version 3.</span>
<br><br><a class="drac-text" href="https://github.com/Sietove-vzdelanie/sietovevzdelanie-web/blob/main/LICENSE">ODKAZ NA LICENCIU</a>
  </div>
  <center><button aria-current={$page.url.pathname === '/' ? 'page' : undefined} on:click={redirect} style="margin-top: 1em; margin-left:1em; width:6em" class="drac-btn drac-bg-purple drac-m-sm drac-btn-lg">
	SPÄŤ</button></center>
</div>

