<script lang="ts">
	import logo from '$lib/images/visitingCard.jpg';

	export let name: string;
</script>

<a href="/design/visting" class="flex flex-col  items-center p-5 ">
	<img src={logo} alt="" />
	<div class="my-4">{name}</div>
</a>
