<script>
	let name = 'Stranger';
	let message = "You are on Earth";

	const handleClick = () =>{
			message = 'You are on Earth';
	}
	const handleInput =(e) =>{
			message = e.target.value;
	}
</script>

<main>
   <h2> Mmmm type in something <i>{name}</i></h2>
   <h3> {message}.</h3>
   <div class="border-5">Where are you from : <input type="text" on:input="{handleInput}"></div>
   <p><button on:click={handleClick}> Be realisitc </button></p>
</main>

<style>
	main {
		text-align: center;
		padding: 1em;
		max-width: 240px;
		margin: 0 auto;
	}

	h1 {
		color: #ff3e00;
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