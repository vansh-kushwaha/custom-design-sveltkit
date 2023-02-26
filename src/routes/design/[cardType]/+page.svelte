<script lang="ts">
	import CustomInput from '$lib/components/form/CustomInput.svelte';
	import CustomSelect from '$lib/components/form/CustomSelect.svelte';
	import CustomTextArea from '$lib/components/form/CustomTextArea.svelte';

	const productOption = ['1 side', '2 side'];
</script>

<div>
	<h1>Add Order</h1>

	<div>
		<form action="">
			<CustomInput label={'Order Name'} />
			<CustomSelect options={productOption} label={'Choose Product'} />

			<div class="grid grid-cols-2 gap-4 ">
				<CustomInput label={'Name'} />
				<CustomInput label={'Mobile No'} />
				<CustomInput label={'Name'} />
				<CustomInput label={'Mobile No'} />

				<CustomInput label={'Firm Name'} />
				<CustomTextArea label={'Address'} rows={2} />
			</div>

			<CustomTextArea label={'Description'} />

			<div class="mb-6">
				<label class="block mb-2 text-sm font-medium text-gray-900 dark:text-white" for="large_size"
					>Large file input</label
				>
				<input
					class="block w-full text-lg text-gray-900 border border-gray-300 rounded-lg cursor-pointer bg-gray-50 dark:text-gray-400 focus:outline-none dark:bg-gray-700 dark:border-gray-600 dark:placeholder-gray-400"
					id="large_size"
					type="file"
				/>
			</div>

			<div class="flex items-center justify-center w-full">
				<label
					for="dropzone-file"
					class="flex flex-col items-center justify-center w-full h-64 border-2 border-gray-300 border-dashed rounded-lg cursor-pointer bg-gray-50 dark:hover:bg-bray-800 dark:bg-gray-700 hover:bg-gray-100 dark:border-gray-600 dark:hover:border-gray-500 dark:hover:bg-gray-600"
				>
					<div class="flex flex-col items-center justify-center pt-5 pb-6">
						<svg
							aria-hidden="true"
							class="w-10 h-10 mb-3 text-gray-400"
							fill="none"
							stroke="currentColor"
							viewBox="0 0 24 24"
							xmlns="http://www.w3.org/2000/svg"
							><path
								stroke-linecap="round"
								stroke-linejoin="round"
								stroke-width="2"
								d="M7 16a4 4 0 01-.88-7.903A5 5 0 1115.9 6L16 6a5 5 0 011 9.9M15 13l-3-3m0 0l-3 3m3-3v12"
							/></svg
						>
						<p class="mb-2 text-sm text-gray-500 dark:text-gray-400">
							<span class="font-semibold">Click to upload</span> or drag and drop
						</p>
						<p class="text-xs text-gray-500 dark:text-gray-400">
							SVG, PNG, JPG or GIF (MAX. 800x400px)
						</p>
					</div>
					<input id="dropzone-file" type="file" class="hidden" />
				</label>
			</div>

			<button>Submit</button>
		</form>
	</div>
</div>
