<script>
	let text = 'Sample Text, <h5>edit it here<h5>';
	function showText () {
		console.log(text);
		alert(text)
	}
</script>


<main>
	
	<h1>Write your text below</h1>

	<input bind:value={text}>
	<button on:click={showText}>
		Show on console and alert
	</button>
	
	<hr>
	
	<h5> The text is: </h5>
	
	<p>{text}</p>
	
	<br>	
	<hr>
	<br>
	
	<h5>Showing as HTML component:</h5>
	<p>{@html text}</p>
	
	<br>
</main>


<style>
	p {
		font-family:Helvetica;
	}
</style>
