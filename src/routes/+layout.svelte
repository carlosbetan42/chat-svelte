<script lang="ts">
	import Logo from '../components/Logo.svelte';

	import '../app.css';
</script>

<!-- <header>Esto es el header</header> -->

<main class="max-w-6xl m-auto px-4 relative">
	<Logo />
	<slot />
</main>
