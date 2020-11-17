<script>

</script>
<style>
	body {
		font-family: "Mulish", sans-serif;
	}

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

	input:not(:checked) ~ #menu-button::before {
		content: "| | |";
	}

	input:checked ~ #menu-button:before {
		content: "|||";
	}


	#menu-checkbox {
		display: none;
	}
	#menu-checkbox:not(:checked) + * + div {
		display: none;
	}

	#welcome {
		text-align: center; 
		font-size: 800;
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
		border-bottom: #FF6347 0.3rem solid;
	}
</style>

<main>
<link rel="preconnect" href="https://fonts.gstatic.com">
<link href="https://fonts.googleapis.com/css2?family=Mulish:wght@500&display=swap" rel="stylesheet">
	<header>
		
		<nav>
			<input id="menu-checkbox" type="checkbox" />
			<label id="menu-button" for="menu-checkbox"></label>
			<div>
				<span id="welcome">Buja</span>
				<></p>
			</div>
		</nav>
	</header>
	<div id="main-content">
		<div id="">
	</div>
</main>