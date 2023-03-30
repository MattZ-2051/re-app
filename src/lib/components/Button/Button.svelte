<script lang="ts">
	export let label: string;
	export let classes: string | undefined = undefined;
</script>

<div class="flex justify-center space-x-2">
	<button
		type="button"
		class={`${classes} inline-block rounded px-6 pt-2.5 pb-2 text-xs font-medium uppercase leading-normal transition duration-150 ease-in-out focus:outline-none`}
	>
		{label}
	</button>
</div>
