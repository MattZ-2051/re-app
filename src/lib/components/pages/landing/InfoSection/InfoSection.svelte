<script lang="ts">
	export let img: string;
	export let title: string;
	export let body: string;
	export let flip = false;
</script>

<div class="flex items-center mt-20 w-full h-full p-12">
	{#if !flip}
		<div class="w-full justify-center items-start h-[400px] flex">
			<div class="bg-black h-24 p-6 w-2/3">
				<h1 class="text-white text-center text-5xl">{title}</h1>
				<p class="text-lg text-center mt-16">
					{body}
				</p>
			</div>
		</div>

		<img src={img} alt="landing-bg" class="h-[400px] w-full" />
	{:else}
		<img src={img} alt="landing-bg" class="h-[400px] w-full" />
		<div class="w-full justify-center items-start h-[400px] flex">
			<div class="bg-black h-24 p-6 w-2/3">
				<h1 class="text-white text-center text-5xl">{title}</h1>
				<p class="text-lg text-center mt-16">
					{body}
				</p>
			</div>
		</div>
	{/if}
</div>
