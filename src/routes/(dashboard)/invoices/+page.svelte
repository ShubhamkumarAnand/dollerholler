<script lang="ts">
	import CircledAmount from '$lib/components/CircledAmount.svelte';
	import ThreeDots from '$lib/components/Icon/ThreeDots.svelte';
	import View from '$lib/components/Icon/View.svelte';
	import Search from '$lib/components/Search.svelte';
	import Tag from '$lib/components/Tag.svelte';
</script>

<svelte:head>
	<title>Invoice | The Doller Holler</title>
</svelte:head>

<div>
	<!-- header -->
	<div class="mb-16 flex items-center justify-between">
		<!-- Search Field -->
		<Search />
		<!-- New Invoice -->
		<div>
			<button
				class="relative translate-y-0 whitespace-nowrap rounded-lg bg-lavenderIndigo px-10 py-3 font-sansSerif text-xl font-black text-white shadow-colored transition-all hover:-translate-y-2 hover:shadow-coloredHover"
				>+ Invoice</button
			>
		</div>
	</div>

	<!-- List of invoices -->
	<div>
		<!-- header -->
		<div class="table-header invoice-table text-daisyBush">
			<h3>Status</h3>
			<h3>Issue Date</h3>
			<h3>ID</h3>
			<h3>Client</h3>
			<h3>Amount</h3>
			<div />
			<div />
		</div>
		<!-- invoices -->
		<div class="invoice-table items-center rounded-lg bg-white py-6 shadow-tableRow">
			<div><Tag label="draft" /></div>
			<div class="font-lg">12/12/23</div>
			<div class="font-lg">1234</div>
			<div class="font-lg font-bold">Compressed.fm</div>
			<div class="font-lg font-mono font-bold">$543.55</div>
			<div class="font-lg center">
				<a href="/viewMore" class="text-pastelPurple hover:text-daisyBush"><View /></a>
			</div>
			<div class="font-lg center">
				<button class="text-pastelPurple hover:text-daisyBush"><ThreeDots /></button>
			</div>
		</div>
	</div>
</div>

<CircledAmount label="Total" amount="$1,343.44" />

<style lang="postcss">
	.table-header {
		@apply text-xl font-black leading-snug;
	}
</style>
