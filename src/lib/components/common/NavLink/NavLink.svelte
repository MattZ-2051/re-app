<script lang="ts">
	import './NavLink.css';
	$: showLine = false;
	export let label: string;
	export let to: string;
	export let classes: string | undefined = undefined;
</script>

<div class={classes}>
	<div
		class={`navLink hover:cursor-pointer flex flex-col text-sm sm:text-base h-full`}
		on:mouseenter={() => (showLine = true)}
		on:mouseleave={() => (showLine = false)}
	>
		<a href={to}>{label}</a>
		{#if showLine}
			<span class={`z-10 bg-slate-500 inline-block h-[2px] line mt-1`} />
		{:else}
			<span class="w-full bg-transparent h-[2px]" />
		{/if}
	</div>
</div>
