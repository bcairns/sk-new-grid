<script>
	import MaxWidthAndPadding from './MaxWidthAndPadding.svelte';
</script>

<div class="fixed top-0 left-0 right-0 bottom-0 pointer-events-none z-50" style="opacity:0.05">
	<MaxWidthAndPadding class="h-full grid gap grid-cols-4 md:grid-cols-8 lg:grid-cols-12">
		{#each { length: 4 } as _, index}
			<div class="bg-green" />
		{/each}
		{#each { length: 4 } as _, index}
			<div class="bg-green hidden md:block" />
		{/each}
		{#each { length: 4 } as _, index}
			<div class="bg-green hidden lg:block" />
		{/each}
	</MaxWidthAndPadding>
</div>
