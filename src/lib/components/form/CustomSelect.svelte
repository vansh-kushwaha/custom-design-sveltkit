<script lang="ts">
	export let label: string;
	export let options: string[];
</script>

<div class="mb-6">
	<label for="countries" class="block mb-2 text-sm font-medium text-gray-900 dark:text-white"
		>{label}</label
	>
	<select
		id="countries"
		class="bg-gray-50 border border-gray-300 text-gray-900 text-sm rounded-lg focus:ring-blue-500 focus:border-blue-500 block w-full p-2.5 dark:bg-gray-700 dark:border-gray-600 dark:placeholder-gray-400 dark:text-white dark:focus:ring-blue-500 dark:focus:border-blue-500"
	>
		<option selected>Choose a Product</option>
		{#each options as o}
			<option value={o}> {o} </option>
		{/each}
	</select>
</div>
