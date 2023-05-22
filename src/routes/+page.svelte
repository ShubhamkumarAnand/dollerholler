<script>
	import { FormatText } from '$utils/FormatText';
</script>

<h1 class="text-3xl font-bold">Welcome to the Svelte World.</h1>

{FormatText('Jack')}

<style lang="postcss">
	:global(html) {
		background-color: theme(colors.gray.100);
	}
</style>
