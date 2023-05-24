<script lang="ts">
	import Search from './Icon/Search.svelte';
</script>

<div class="relative flex w-full items-baseline gap-6">
	<div class="mr-2 mt-auto text-pastelPurple">
		<Search height={32} width={32} />
	</div>
	<input
		type="text"
		placeholder="Search by Keyword"
		name="search"
		class="w-72 border-b-2 border-dashed border-b-pastelPurple bg-transparent font-sansSerif text-xl text-black outline-none focus:border-solid focus:border-b-lavenderIndigo"
	/>
	<button class="font-sansSerif text-xl font-black text-pastelPurple">Search</button>
</div>
