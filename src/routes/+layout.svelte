<div class="main-layout">
	<nav>
		<a href="/" class="nav-logo">Sentiment Sage</a>
		<div class="nav-links">
			<a href="/sign-in">Sign in</a>
			<a href="/sign-up">Register</a>
		</div>
	</nav>

	<main>
		<slot />
	</main>

	<footer>
		Copyright 2023 Sentiment Sage

		<div class="footer-links">
			<a
				href="https://www.linkedin.com/in/stephenfillers/"
				target="_blank"
				rel="noopener noreferrer"><i class="fab fa-linkedin" /></a
			>
			<a href="https://github.com/stephenfillers" target="_blank" rel="noopener noreferrer"
				><i class="fab fa-github" /></a
			>
		</div>
	</footer>
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
		background-color: var(--secondary-color);
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
		margin: 0 0.5rem 0 0;
		border: 1px solid var(--light-color);
		padding: 0.5rem 1rem;
	}

	.nav-links > a:hover {
		background-color: var(--light-color);
		color: var(--dark-color);
	}

	footer {
		height: 60px;
		background-color: var(--dark-color);
		color: #fff;
		display: flex;
		align-items: center;
		justify-content: space-between;
		padding: 0 1rem;
	}

	.footer-links > a {
		color: #fff;
		text-decoration: none;
		margin-left: 0.5rem;
	}
</style>
