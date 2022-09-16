<script>
	import { scale } from 'svelte/transition';
	export let refresh = '';
</script>

{#key refresh}
	<div in:scale={{ duration: 250, delay: 0, start: 0.7 }} out:scale={{ duration: 250 }}>
		<slot />
	</div>
{/key}
