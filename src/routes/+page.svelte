<script lang="ts">
	import landingBg from '$lib/assets/landing-bg.png';
	import Button from '$lib/components/Button/Button.svelte';
</script>

<div class="relative">
	<img
		src={landingBg}
		alt="landing-bg"
		class="h-[500px] object-cover w-full bg-local shadow-xl opacity-60 absolute -z-50"
	/>
	<div class="w-full h-[500px] flex p-12 text-white font-light items-center justify-center z-10">
		<div class="text-center">
			<p class="text-5xl">Explore Homes in Boise</p>
			<p class="text-3xl py-4">dolor sit amet</p>
			<p class="text-5xl">Ut enim ad</p>
			<Button
				label="Explore Homes"
				classes="bg-transparent text-white border-2 mt-12 hover:scale-110"
			/>
		</div>
	</div>
</div>
