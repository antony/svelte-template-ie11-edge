<script>
	export let disabled;
</script>

<main>
	<button {disabled}>Maybe Disabled</button>
	<button disabled={disabled}>Maybe Disabled</button>

	<p>Disabled it?</p>
	<label>
		<input type="radio" bind:group={disabled} value={true} />
		Yes
	</label>
	<label>
		<input type="radio" bind:group={disabled} value={false} />
		No
	</label>
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