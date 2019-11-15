<script>
	import Nav from '../components/Nav.svelte';

	export let segment;
</script>

<style lang="scss" global>
 @import "./global/styles/global.scss";

	body {
		margin: 0;
		font-family: Roboto, -apple-system, BlinkMacSystemFont, Segoe UI, Oxygen, Ubuntu, Cantarell, Fira Sans, Droid Sans, Helvetica Neue, sans-serif;
		font-size: 14px;
		line-height: 1.5;
		color: #333;
		@media (min-width: 400px) {
			font-size: 16px;
		}
	}

	main {
		position: relative;
		max-width: 56em;
		background-color: white;
		padding: 2em;
		margin: 0 auto;
		box-sizing: border-box;
	}
</style>

<Nav {segment}/>

<main>
	<slot></slot>
</main>