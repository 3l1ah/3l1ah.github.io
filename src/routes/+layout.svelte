<script lang="ts">
	import '../app.css';
	import namegames from '$lib/namegames.svg';
	import Squares from '$lib/Squares.svelte';
	let { children } = $props();
</script>

<div class="overscroll-none font-inconsolata text-white">
	<div class="fixed top-0 left-0 bg-gradient-to-b from-black right-0 z-50 flex p-3">
		<img class="size-10" src={namegames} />
	</div>
	{@render children()}
	<div class="border-t items-center gap-3 p-6 border-amber-600 mt-6 flex">
		<img class="size-8" src={namegames} />
		<p class="font-mangold">namegames</p>
	</div>
</div>
