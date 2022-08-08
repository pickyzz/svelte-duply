<script lang='ts'>
	import '../app.css';
	import Kofi from '$lib/components/Kofi.svelte'
	import ShareButton from '$lib/components/ShareButton.svelte'

	const url = 'https://pickyzz.dev'
	const title = 'Sveltekit Template'
	
</script>

<main>
	<Kofi name="pickyzz" label="Buy me Coffee" />
	<ShareButton {url} {title} />
	<slot />
</main>
