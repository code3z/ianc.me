<script>
	import PageTransition from '$lib/PageTransition.svelte';
	import '../app.css';
	import { page, navigating } from '$app/stores';
</script>

<PageTransition refresh={$page.url.href}>
	<main class="sm:p-8 p-4 max-w-6xl mx-auto pt-16" style:display={$navigating ? 'none' : 'block'}>
		<slot />
	</main>
</PageTransition>
