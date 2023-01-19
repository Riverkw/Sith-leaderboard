<script>
	import Header from './Header.svelte';
	import './styles.css';
</script>

<div class="app bg-slate-800 min-h-screen">
	<Header />

	<main>
		<slot />
	</main>

	<footer>
	</footer>
</div>
