<script lang="ts">
	import NavLink from '$lib/components/common/NavLink/NavLink.svelte';
	import reLogo from '$lib/assets/images/re-logo.png';
</script>

<nav class="h-20 bg-white w-full flex justify-between px-12 items-center text-black">
	<img src={reLogo} alt="" class="w-16 h-16" />
	<div class="flex items-center">
		<NavLink to="/" label="Home" classes="mr-6" />
		<NavLink to="pre-approval" label="Pre Approval" classes="mr-6" />
		<NavLink to="payment-calculator" label="Payment Calculator" classes="mr-6" />
		<NavLink to="class" label="Free Home Buyer Class" classes="mr-6" />
		<NavLink to="how-to" label="How To Buy A Home" classes="mr-6" />
		<NavLink to="faq" label="FAQ" classes="mr-6" />
	</div>
</nav>
