<script lang="ts">
	import bgVid from '$lib/bgsneak.mp4';
	import SectionTag from './SectionTag.svelte';
</script>

<svelte:head>
	<title>Home - namegames</title>
</svelte:head>
<div class="flex items-end lg:items-center relative h-screen justify-center md:justify-end">
	<div
		class="absolute z-20 top-0 left-0 right-0 bottom-0 h-full w-full bg-gradient-to-b to-95% to-[#0d0b02]"
	></div>
	<video
		autoplay
		muted
		loop
		playsinline
		class="absolute z-10 top-0 right-0 bottom-0 left-0 h-full w-full object-cover"
		><source src={bgVid} /></video
	>
	<div class="md:text-right text-center z-20 pb-20 space-y-6 px-16 w-full">
		<p class="font-foundation-gothic text-4xl md:text-6xl uppercase">The Foundation</p>
		<p>A reimagination of the Roblox game DOORS.</p>
	</div>
</div>
<div
	class="flex flex-col w-4/5 md:flex-row md:items-center items-baseline justify-center h-screen mx-8 gap-6"
>
	<SectionTag>About Us</SectionTag>
	<p class="text-3xl md:text-5xl">
		We are a development team that create <span class="italic text-orange-400 engaging"
			>engaging</span
		>, high quality games on Roblox.
	</p>
</div>
<div class="flex flex-col md:flex-row md:items-center items-baseline h-screen mx-6">
	<div class="flex flex-col items-start md:mx-8">
		<SectionTag>Latest Update</SectionTag>
		<p class="font-mangold italic text-5xl mb-6 md:text-5xl">Sneak Peek #7</p>
		<p class="text-xl opacity-50 mb-3">
			The latest sneak peek for The Foundation, featuring The Observatory.
		</p>
	</div>
	<iframe
		class="w-full h-full"
		src="https://www.youtube.com/embed/XPmnNFSFxrg"
		title="THE FOUNDATION - SNEAK PEEK #7 (THE OBSERVATORY)"
		frameborder="0"
		allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
		referrerpolicy="strict-origin-when-cross-origin"
		allowfullscreen
	></iframe>
</div>

<style>
	.engaging {
		text-shadow: 0 3px 20px oklch(0.75 0.183 55.934);
	}
	.foundation-glow {
		text-shadow: 0 2px 7px oklch(100% 0 0);
	}
</style>
