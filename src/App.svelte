<script>
	import Display from './Display.svelte';

	let displayText = '';
	let keys = [
		0,1,2,3,4,
		5,6,7,8,9
	]

</script>

<style>
	div, header {
		max-width: 768px;
		margin: auto;
	}

	div {
		border: 1px solid black;
	}

	header {
		padding: 0.5em;
		text-align: center;
		font-size: 1.5em;
		background: #000;
		color: #fff;
	}
</style>

<header>Ninja Calculator</header>

<div>
	<Display {displayText} />
</div>
