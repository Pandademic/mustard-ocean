<script>
	export let text;
	export let moveUp;
</script>

<!-- svelte-ignore a11y-missing-content -->
{#if moveUp == 'true'}
	<h3 id="fire-text" class="slide-up">{text}</h3>
{:else}
	<h3 id="fire-text">{text}</h3>
{/if}

<style>
	@import url('https://fonts.googleapis.com/css2?family=Caesar+Dressing&display=swap');
	#fire-text {
		font-family: “Open Sans”, sans-serif;
		color: #f5f5f5;
		text-shadow: 0px -2px 4px #fff, 0px -2px 10px #ff3, 0px -10px 20px #f90, 0px -20px 40px #c33;
		font-size: 100px;
		font-family: 'Caesar Dressing', cursive;
	}
	@keyframes moveUp {
		0% {
			transform: translateY(500px);
		}
		100% {
			transform: translateY(0px);
		}
	}
	.slide-up {
		animation: moveUp 1s ease-in-out;
		animation-delay: 10ms;
	}
</style>
