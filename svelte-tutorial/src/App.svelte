<script>
import Nested from "./Nested.svelte";
	export let name;
	let world = "world~";
	let sentence = `this <b>string</b> is very easy`;
	let count = 0;
	$: doubled = count * 2
	function handleClick(){
		count += 1;
	}

</script>

<main>
	<h1>Hello {world}!</h1>
	<p>Visit the <a href="https://svelte.dev/tutorial">Svelte tutorial</a> to learn how to build Svelte apps.</p>
	<p>{@html sentence}</p> 

	<button on:click={handleClick}>
		Clicked {count} {count === 1? 'time' : 'times'}
	</button>
	<p>{count} doubled is {doubled}</p>
						   <!-- count * 2와 동일한 의미 -->

</main>
<Nested/>
<h1>Hello {world}!</h1>

<style>
	main {
		text-align: center;
		padding: 1em;
		max-width: 240px;
		margin: 0 auto;
	}

	main h1 {
		color: #ff3e00;
		text-transform: uppercase;
		font-size: 4em;
		font-weight: 100;
	}

	h1 {
		text-align: center;
		color: black;
		text-transform: uppercase;
		font-size: 4em;
		font-weight: 100;
	}

	@media (min-width: 640px) {
		main {
			max-width: none;
		}
	}
</style>