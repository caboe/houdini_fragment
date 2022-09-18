<script lang="ts">
	import type { PageData } from '$houdini/types/src/routes/$houdini';
	export let data: PageData;

	$: ({ Country } = data);
</script>

<h1>Welcome to SvelteKit</h1>
<p>Visit <a href="https://kit.svelte.dev">kit.svelte.dev</a> to read the documentation</p>

<h5>{$Country.data?.country?.name}</h5>
