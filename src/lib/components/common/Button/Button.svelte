<script lang="ts">
	import './Button.css';
	import type { ButtonVariant, Variants } from './types';

	export let label: string;
	export let classes: string | undefined = undefined;
	export let variant: ButtonVariant;

	const variants: Variants = {
		primary: 'button',
		secondary:
			'inline-block rounded px-6 pt-2.5 pb-2 text-xs font-medium uppercase leading-normal transition duration-150 ease-in-out focus:outline-none bg-transparent border-2'
	};
</script>

<!-- <div class="flex justify-center space-x-2"> -->
<button type="button" class={`${classes}  focus:outline-none ${variants[variant]}`}>
	{label}
	<span />
</button>
<!-- </div> -->
