<script>
	export let message;
	export let status;
</script>

<h1>{status}: {message}</h1>
<title>mustard: {message}</title>

<style>
	@import url('https://fonts.googleapis.com/css2?family=Mouse+Memoirs&display=swap');
	:global(body) {
		background-color: #ffdb58;
		color: white;
		text-align: center;
	}
	* {
		font-family: 'Mouse Memoirs', sans-serif;
		letter-spacing: 3px;
		font-size: 100px;
	}
</style>
