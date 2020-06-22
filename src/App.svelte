<script>
// components
import Wave from './components/Wave.svelte'

let bookTitle = "Itchy Scrotum"
let waving = false
</script>

<style>
	label {
		position: absolute;
		top: 1em;
		left: 1em;
		font-size: 0.7em;
	}
</style>

<header>
	<h1>HEMINGWAYOVÁTORO-ROTÁTOR™</h1>

	<label for="waving">
		<input type="checkbox" id="waving" bind:checked={waving}>
		waving
	</label>
</header>

<main>
	<h2>{bookTitle}</h2>

	<section class="controls">
		<!--  -->
	</section>
</main>

<footer class="water">
	<Wave where="back" animation="big" {waving} />
	<Wave where="middle" animation="tiny" {waving} />
	<img class="hem" src="./assets/hemingway.png" alt="my boy ernest" />
	<Wave where="front" animation="small" {waving} />
</footer>