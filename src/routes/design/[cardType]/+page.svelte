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

			<button>Submit</button>
		</form>
	</div>
</div>
