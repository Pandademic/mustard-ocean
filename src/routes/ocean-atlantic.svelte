<script>
	import Fire from '../lib/Fire.svelte';
</script>
<title>mustard: the atlantic ocean</title>
<h2 class="slide-left">
	How many packets of Djoin mustard would it take to fill the atlantic ocean?
</h2>
<p>(This page is animated and things will slide in)</p>
<br />
<br />
<br />
<Fire text="That's a burning question" moveUp="true"/>
<h1 class="slide-left">1.7984133e22 packets, that's how many.</h1>
<style>
	@import url('https://fonts.googleapis.com/css2?family=Mouse+Memoirs&display=swap');
	:global(body) {
		background-color: #ffdb58;
		color: white;
		text-align: center;
	}
	h2 {
		font-size: 35px;
	}
	h1 {
		font-size: 90px;
	}
	.slide-left{
		animation: moveToRight 1s ease-in-out;
        animation-delay: 10ms;
	}
	@keyframes moveToRight {
            0% {	
                transform: translateX(500px);
            }
            100% {
                transform: translateX(0px);
            }
	}
	*{
		font-family: 'Mouse Memoirs', sans-serif;
	}
</style>
