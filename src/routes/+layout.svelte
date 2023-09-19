<script>
	import '../app.postcss';
</script>

<main class="container">
	<slot />
</main>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
	}

	.container {
		width: 100%;
		max-width: 768px;
		padding: 10px 20px;
		margin: 0 auto;
		display: flex;
		align-items: center;
		justify-content: center;
		min-height: 100vh;
	}
</style>
