<script>
	import Card from '$lib/components/Card.svelte';

	const products = [
		{
			label: 'Visiting Card Design'
		},
		{
			label: 'Logo Design'
		},
		{
			label: 'Folder Design'
		},
		{
			label: 'Poster/Banner Design'
		},
		{
			label: 'Social Media Post Design'
		}
	];
</script>

<div>
	<h1 class="text-center ">Designing</h1>
	<h2 class="text-center mt-3 mb-10">List Of Products</h2>

	<div class="grid grid-cols-3 gap-8">
		{#each products as p}
			<Card name={p.label} />
		{/each}
	</div>
</div>
