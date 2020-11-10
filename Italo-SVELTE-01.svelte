<script>
		let storeForm = {};
	
	function alerts() {
		alert(storeForm.name);
		alert(storeForm.address);
	};
</script>

<div>
	<form>
		<label for="Nome">Nome da loja</label>
		<input type="text" name="nome" bind:value={storeForm.name} placeholder="Insira o nome:" required>
		<label for="Endereço">Endereço da loja</label>
		<input type="text" name="endereço" bind:value={storeForm.address} placeholder="Insira o endereço:" required>
		<button on:click|preventDefault={()=> alerts()}>Enviar formulário</button>
	</form>
	
</div>
