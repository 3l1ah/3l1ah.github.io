<script lang="ts">
	import '../app.css';

	import namegames from '$lib/namegames.svg';
	import discord from '$lib/discord.svg';

	import Squares from '$lib/Squares.svelte';
	let { children } = $props();
</script>

<div class="overscroll-none font-inconsolata text-white">
	<div class="fixed top-0 left-0 bg-gradient-to-b justify-between from-black right-0 z-50 flex p-3">
		<img class="size-10" src={namegames} />
		<div class="flex gap-2">
			<a href="https://discord.gg/namegames"><img class="size-10" src={discord} /></a>
		</div>
	</div>
	{@render children()}
	<div class="border-t items-center gap-3 p-6 border-amber-600 mt-6 flex">
		<img class="size-8" src={namegames} />
		<p class="font-mangold">namegames</p>
	</div>
</div>
