<script lang="ts">
	let { children } = $props();
</script>

<p
	class="uppercase height mb-2 mt-0 px-[6px] tracking-wide text-[#0d0b02] text-base/tight bg-amber-600 text-nowrap"
>
	{@render children()}
</p>
