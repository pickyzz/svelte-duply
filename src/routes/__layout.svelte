<script lang='ts'>
	import '../app.css';
	import Kofi from '$lib/components/Kofi.svelte'
	import ShareButton from '$lib/components/ShareButton.svelte'
	import { themeChange } from 'theme-change'
	import { onMount } from 'svelte'
	import Darkmode from '$lib/components/Darkmode.svelte'

	onMount(() => {
		themeChange(false)
	})

	const url = 'https://pickyzz.dev'
	const title = 'Sveltekit Template'
	
</script>

<main>
	<Darkmode />
	<Kofi name="pickyzz" label="Buy me Coffee" />
	<ShareButton {url} {title} />
	<slot />
</main>
