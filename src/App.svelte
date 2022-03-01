<script>
	let time = [7, 0, 0]
	let hours = time[0];
	let minutes = time[1];
	let seconds = time[2];
	
	if (hours > 9) {
		hours = time[0].toString();
	}else {
		hours =  "0"+ time[0].toString();
	}

	if (minutes > 9) {
		 minutes = time[1].toString();
	}else {
		 minutes = "0" + time[1].toString();
	}

	if (seconds > 9) {
		 seconds = time[2].toString();
	}else {
		 seconds = "0" + time[2].toString();
	}
</script>

<main>
	<div class="container">
		<div class="base-container">
			<h1 class="time">{hours+ ":" +minutes + ":" + seconds}</h1>
			<div class="buttons-container">
				<button class="play btn">Play</button>
			<button class="reset btn">Reset</button>
			<button class="stop btn">Stop</button>
			</div>		
		</div>
		
		
	</div>
</main>

<style>
	@import url('https://fonts.googleapis.com/css2?family=Poppins:wght@700&display=swap');
	* {
		padding: 0;
		margin: 0;
		box-sizing: border-box;
		font-family: 'Poppins', sans-serif;
		
	}
	.container {
		margin: 0 auto;
		width: 100%;
		height: 80vh;
		display: flex;
		align-items: center;
		justify-content: center;
	}
	.base-container {
		text-align: center;
	}
	.time {
		color: blue;
	}
	.btn {
		padding: 0.6em 1.5em;
		margin: 0 1em;
		border-radius: 10px;
		border: none;
		background-color: 	aqua;
		color: white;
		transition: 1s;
	}
	.btn:hover {
		background-color: rgb(101, 250, 250);
	}
</style>