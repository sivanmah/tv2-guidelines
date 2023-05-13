<script>
	import Navbar from './components/Navbar/Navbar.svelte';
	import Guidelines from './components/Guidelines/Guidelines.svelte';
	import Calculator from './components/Calculator/Calculator.svelte';
</script>

<svelte:head>
	<title>Web Sustainability Guidelines</title>
</svelte:head>

<div class="container">
	<div class="navbar">
		<Navbar />
	</div>
	<div class="content">
		<Guidelines />
	</div>
	<div class="calculator">
		<Calculator />
	</div>
</div>

<style>
	:global(body) {
		background-color: #282828;
		color: #f0f0f0;
		font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Helvetica, Arial, sans-serif,
			'Apple Color Emoji', 'Segoe UI Emoji', 'Segoe UI Symbol';
		margin: 0;
	}

	.container {
		display: flex;
		min-height: 100vh;
	}

	.navbar {
		width: 20%;
		min-height: 100vh;
	}

	.content {
		width: 80%;
		padding: 2rem;
	}

	/* Add media queries for responsiveness */
	@media (max-width: 1024px) {
		.navbar {
			width: 30%;
		}
		.content {
			width: 70%;
		}
	}

	@media (max-width: 768px) {
		.container {
			flex-direction: column;
		}
		.navbar {
			width: 100%;
			min-height: auto;
		}
		.content {
			width: 100%;
		}
	}
</style>
