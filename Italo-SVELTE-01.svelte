<script>
	let name;
	let address;
	
	function alerts() {
		let storeForm = {
			"name": name,
			"address": address,
			};
		alert(storeForm.name);
		alert(storeForm.address);
	};
</script>

<div>
	<form method="post" on:submit={alerts}>
		<label for="Nome">Nome da loja</label>
		<input type="text" name="nome" bind:value={name} placeholder="Insira o nome:" required>
		<label for="Endereço">Endereço da loja</label>
		<input type="text" name="endereço" bind:value={address} placeholder="Insira o endereço:" required>
		<button type="submit">Enviar formulário</button>
	</form>
</div>
