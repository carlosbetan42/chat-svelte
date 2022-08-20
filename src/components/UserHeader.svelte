<script lang="ts">
	let anonymousName = '';
	let showAnonymousInput = true;

	const handleAnonymousInput = (e: SubmitEvent) => {
		e.preventDefault();
		// guardamos el anonymousName
	};

	const handleToggleAnonymous = () => {
		showAnonymousInput = !showAnonymousInput;
	};
</script>

<header>
	{#if showAnonymousInput}
		<form on:submit={handleAnonymousInput}>
			<input type="text" placeholder="Indica tu nombre anónimo" />
		</form>
	{:else}
		<button on:click={handleToggleAnonymous} class="py-2 flex items-center gap-1 hover:underline">
			Entrar como anónimo
		</button>
	{/if}
</header>
