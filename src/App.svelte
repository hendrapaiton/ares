<script>
	export let name;
</script>

<main class="container has-text-centered">
	<h1 class="title is-size-1 has-text-primary">Hello {name}!</h1>
	<i class="las la-plane-departure has-text-danger"></i>
	<p class="subtitle is-size-5 has-text-warning">Visit the <a href="https://svelte.dev/tutorial">Svelte tutorial</a> to learn how to build Svelte apps.</p>
</main>

<style>
	i.las.la-plane-departure {
		margin: 0 !important;
		padding: 0 !important;
		font-size: 74pt;
	}
</style>