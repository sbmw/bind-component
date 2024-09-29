<script lang="ts">
	import SimpleComponent from '$lib/Simple.svelte';
	import RunesModeComponent from '$lib/RunesMode.svelte';

	let simpleComponent: SimpleComponent;
	let runesModeComponent: RunesModeComponent;
</script>

<button
	onclick={() => {
		simpleComponent.saySimpleComponent();
	}}>Simple Component</button
>

<button
	onclick={() => {
		runesModeComponent.sayRunesModeComponent();
	}}>Runes Mode Component</button
>

<SimpleComponent bind:this={simpleComponent}></SimpleComponent>
<RunesModeComponent bind:this={runesModeComponent}></RunesModeComponent>
