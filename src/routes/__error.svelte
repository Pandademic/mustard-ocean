<script context="module">
	export function load({ error, status }) {
		return {
			props: {
				message: error.message,
				status // same as status: status
			}
		};
	}
</script>

<script>
	import ErrorScreen from '../lib/screens/ErrorScreen.svelte';
	import NotFoundScreen from '../lib/screens/NotFoundScreen.svelte';

	export let message;
	export let status;
</script>

{#if status == 404}
	<NotFoundScreen />
{:else}
	<ErrorScreen {message} {status} />
{/if}

<style>
	@import url('https://fonts.googleapis.com/css2?family=Mouse+Memoirs&display=swap');
	:global(body) {
		background-color: #ffcb15;
		color: white;
		text-align: center;
	}
	* {
		font-family: 'Mouse Memoirs', sans-serif;
	}
</style>
