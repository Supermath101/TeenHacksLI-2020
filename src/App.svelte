<script>
	let current = null;
	import page from "page";
	import Home from "./Home.svelte"
	import ForgotPasswordPage from "./ForgotPasswordPage.svelte"
	import LoginPage from "./LoginPage.svelte"
	page("/", () => current = Home);
	page("/forgot-password", () => current = ForgotPasswordPage)
	page("/login", () => current = LoginPage)
	page();
</script>

<style>
	main {
		background: #444;
		width: 100%;
		height: 100vh;
		color: #FF6347;
		font-size: 1.5em;
	}
	* {
		margin:0;
		padding:0;
	}

	#menu-button {
		rotate: 90deg;
		display: inline-block;
		user-select: none;
		cursor: pointer;
		margin-left: 1.25rem;
		font-size: 2rem;
		letter-spacing: 0.125em;
	}

	#menu-checkbox:not(:checked) ~ #menu-button::before {
		content: "|||";
	}

	#menu-checkbox:checked ~ #menu-button:before {
		content: "X";
	}


	#menu-checkbox {
		display: none;
	}
	#menu-checkbox:not(:checked) + * + div {
		display: none;
	}

	#text-logo {
		font-size: 3rem;
		font-weight: 600;
	}

	nav {
		display: inline;
	}

	header {
		padding: 0.5rem 0.75rem;
		border-bottom: #FF6347 0.15rem solid;
	}

	#main-content {
		margin: 1rem 2rem;
	}

	header a {
		color: inherit;
		text-decoration: none;
	}
</style>

<main>
	<header>
		<a href="/" id="text-logo">Buja</a>
		<nav>
			<input id="menu-checkbox" type="checkbox" />
			<label id="menu-button" for="menu-checkbox"></label>
			<div>
				<a href="/forgot-password">Forgot Password Page</a><br/>
				<a href="/login">Login</a>
				<!-- TODO: Add list of link within menu here -->
			</div>
		</nav>
	</header>
	<div id="main-content">
		<svelte:component this={current} />
	</div>
</main>
