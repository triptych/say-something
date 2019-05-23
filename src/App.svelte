<script>
	export let name;
	import Counter from './Counter.svelte';
</script>

<style>
	h1 {
		color: purple;
	}
</style>

<h1>Hello {name}!</h1>

<Counter/>
