<script lang="ts">
	import landingBg from '$lib/assets/images/landing-bg.png';
	import testImg1 from '$lib/assets/images/test-img-1.png';
	import testImg2 from '$lib/assets/images/test-img-2.png';
	import Button from '$lib/components/common/Button/Button.svelte';
	import InfoSection from '$lib/components/pages/landing/InfoSection/InfoSection.svelte';
	import StayInTouch from './StayInTouch/StayInTouch.svelte';

	const northEndBody =
		"Boise's Nort End cointains many of the city's older and historic homes. It is known for its tree-lined dries, such as Harrison Boulevard, and for its quiet neighberhoods near the downtown and mountain trail areas - walking distance for most residents. The North End is a gateway to the Boise Foothills, hom eot Camel's Back Park and the historic Hyde Park. If you are looking for charming and convenient, this is the place to be.";
</script>

<div>
	<div class="relative">
		<div class="w-full h-[500px] bg-black opacity-40 absolute -z-10" />
		<img
			src={landingBg}
			alt="landing-bg"
			class="h-[500px] object-cover w-full bg-local shadow-xl absolute -z-50"
		/>
		<div class="w-full h-[500px] flex p-12 text-white font-light items-center justify-center z-10">
			<div class="text-center">
				<p class="text-5xl">Explore Homes in Boise</p>
				<p class="text-3xl py-4">dolor sit amet</p>
				<p class="text-5xl">Ut enim ad</p>

				<Button
					label="Explore Homes"
					variant="secondary"
					classes="bg-transparent text-white border-2 mt-12 hover:scale-110"
				/>
			</div>
		</div>
	</div>
	<div class="mt-24 flex justify-center flex-col items-center">
		<h1 class="text-center text-5xl font-light text-black">Welcome to Boise</h1>
		<div class="w-16 h-[1px] mt-6 bg-black" />
		<h1 class="text-center w-1/2 mt-8 text-2xl font-light text-black">
			Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut
			labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco
			laboris nisi ut aliquip ex ea commodo consequat.
		</h1>
	</div>

	<InfoSection body={northEndBody} title="North End" img={landingBg} />
	<InfoSection body={northEndBody} title="Downtown" img={testImg1} flip={true} />
	<InfoSection body={northEndBody} title="Northwest Boise" img={testImg2} />
	<StayInTouch />
</div>
