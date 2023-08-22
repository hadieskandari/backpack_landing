<script>
	import { page } from '$app/stores';
	import logo from '$lib/images/logo.png';
	import instagram from '$lib/images/instagram.svg';
</script>

<header>
	<div class="corner">
		<a href="https://instagram.com">
			<img src={instagram} alt="instagram" />
		</a>
	</div>

	<div class="corner logo">
		<img src={logo} alt="arfak" />
	</div>
</header>

<style>
	header {
		display: flex;
		justify-content: space-between;
		height: 10vh;
	}

	.corner {
		width: auto;
		height: auto;
		padding: 18px 12px;
	}

	.corner a {
		display: flex;
		align-items: center;
		justify-content: center;
		width: 100%;
		height: 100%;
	}

	.corner a img {
		width: 1.7em;
		height: 1.7em;
	}

	.corner img {
		width: 8em;
		height: 4em;
		object-fit: contain;
	}

	nav {
		display: flex;
		justify-content: center;
		--background: rgba(255, 255, 255, 0.7);
	}

	svg {
		width: 2em;
		height: 3em;
		display: block;
	}

	path {
		fill: var(--background);
	}

	ul {
		position: relative;
		padding: 0;
		margin: 0;
		height: 3em;
		display: flex;
		justify-content: center;
		align-items: center;
		list-style: none;
		background: var(--background);
		background-size: contain;
	}

	li {
		position: relative;
		height: 100%;
	}

	li[aria-current='page']::before {
		--size: 6px;
		content: '';
		width: 0;
		height: 0;
		position: absolute;
		top: 0;
		left: calc(50% - var(--size));
		border: var(--size) solid transparent;
		border-top: var(--size) solid var(--color-theme-1);
	}

	nav a {
		display: flex;
		height: 100%;
		align-items: center;
		padding: 0 0.5rem;
		color: var(--color-text);
		font-weight: 700;
		font-size: 0.8rem;
		text-transform: uppercase;
		letter-spacing: 0.1em;
		text-decoration: none;
		transition: color 0.2s linear;
	}

	a:hover {
		color: var(--color-theme-1);
	}

	.logo {
		padding-top: 8px;
	}
</style>
