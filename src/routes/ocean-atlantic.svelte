<script>
	import Fire from '../lib/Fire.svelte';
</script>
<title>mustard: the atlantic ocean</title>
<h1 class="slide-left">
	How many packets of Djoin mustard would it take to fill the atlantic ocean?
</h1>
<p>(This page is animated and things will slide in)</p>
<br />
<br />
<br />
<Fire text="That's a burning question" moveUp="true"/>
<style>
	@import url('https://fonts.googleapis.com/css2?family=Montserrat:wght@600&display=swap');
	:global(body) {
		background-color: #ffdb58;
		color: white;
		text-align: center;
	}
	h1 {
		font-size: 25px;
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
	#answer{
		font-family: 'Montserrat', sans-serif;
	}
</style>
