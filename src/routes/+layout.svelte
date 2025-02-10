<script lang="ts">
	import type { Snippet } from 'svelte';
    import '../lib/default-hfl.css'

    const {children}: {
        children: Snippet
    } = $props()
</script>

<div class="app">
    {@render children()}
</div>

<style>
    .app {
		display: flex;
		flex-direction: column;
		min-height: 100vh;
        background-color: var(--background-color);
        padding: 20px;
        align-items: center;
	}
</style>