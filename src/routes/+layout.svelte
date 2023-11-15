<script>
	import '../app.scss';
	import MaxWidthAndPadding from "./MaxWidthAndPadding.svelte";
	import GridOverlay from "./GridOverlay.svelte";
</script>

<header class="bg-gray-900 py-8">
	<MaxWidthAndPadding class="flex gap justify-between">
		<div class="">Header</div>
		<div class="">Header</div>
	</MaxWidthAndPadding>
</header>

<main>
	<slot />
</main>

<footer class="bg-gray-200 py-16 text-white">
	<MaxWidthAndPadding class="flex gap justify-between">
		<div class="">Footer</div>
		<div class="">Footer</div>
	</MaxWidthAndPadding>
</footer>

<GridOverlay />