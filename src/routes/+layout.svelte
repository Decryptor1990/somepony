<script>
	import '../app.scss';

	/** @type {{children: import('svelte').Snippet}} */
	let { children } = $props();
</script>

<main class="w-full">
  {@render children()}
</main>
