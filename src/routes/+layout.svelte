<script>
	import '../styles/global.css';
</script>

<div class="main-layout">
	<nav>
		<a href="/" class="nav-logo">Sentiment Sage</a>
		<div class="nav-links">
			<a href="/">Home</a>
			<a href="/about">About</a>
		</div>
	</nav>

	<main>
		<slot />
	</main>

	<footer>Copyright 2023 Sentiment Sage</footer>
</div>

<style>
	.main-layout {
		min-height: 100svh;
		display: grid;
		grid-template-rows:
			auto
			1fr
			auto;
	}

	nav {
		height: 60px;
		background-color: #2e1f42;
		color: #fff;
		margin: 0;
		padding: 0;
		display: flex;
		align-items: center;
		justify-content: space-between;
	}

	.nav-logo {
		font-family: sans-serif;
		font-size: 1.2rem;
		margin: 0 1rem;
		color: #fff;
		text-decoration: none;
	}

	.nav-links > a {
		color: #fff;
		text-decoration: none;
		margin: 0 1rem 0 0;
	}

	main {
		padding: 1rem;
	}

	footer {
		height: 60px;
		background-color: #2e1f42;
		color: #fff;
		display: flex;
		align-items: center;
		padding: 0 1rem;
	}
</style>
