<script>
	import welcome from '$lib/images/text.svg';
	import backpack from '$lib/images/backpack.png';
	import hashtag from '$lib/images/hashtag.svg';
</script>

<svelte:head>
	<title>یک کلیک، یک کوله</title>
	<meta name="description" content="Svelte demo app" />
</svelte:head>

<div class="welcome-container">
	<section>
		<h1 class="mb-0">
			<span class="welcome">
				<img src={welcome} alt="Welcome" width="310px" height="47px" />
			</span>
		</h1>

		<h2 class="welcome-description">
			<span>
				با وارد کردن اسمتون و یک کلیک می‌تونید بانیِ مهر امسال باشید و در تامین ۱۰،۰۰۰ کوله‌پشتی با
				لوازم‌التحریر یک سال تحصیلی شریک بشید.
			</span>
		</h2>

		<div>
			<img src={backpack} alt="backpack" width="268px" height="220px" />
		</div>

		<div class="w-100 mt-2">
			<input type="text" autocomplete="given-name" placeholder="اسمت رو وارد کن" />
		</div>
		<div class="mt-1">
			<button>! کـلـیک کنیـد</button>
		</div>

	
		<div class="alert-rectangle">
			<div class="hashtag mt-2">
				<img src={hashtag} alt="hashtag" />
			</div>
	
			<span>
				هدف کمپین مهر،بانی میخواهد سال ۱۴۰۲، تامین و توزیع ۱۰،۰۰۰ کوله‌پشتی برای کودکان بازمانده از
				تحصیل کشور می‌باشد.
			</span>
		</div>
	</section>
</div>

<style>
	.welcome-container {
		min-height: 90vh;
		height: 100%;
		width: 100%;
		padding: 0;
		background: url('../lib/images/background.png');
		background-size: cover;
		padding: 0;
	}
	section {
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;
		flex: 0.6;
		padding: 0 40px;
	}

	h1 {
		width: 100%;
	}

	.welcome {
		display: block;
		position: relative;
		width: 100%;
		height: 0;
		padding: 0 0 calc(100% * 495 / 2048);
	}

	.welcome img {
		position: absolute;
		width: 100%;
		height: 100%;
		top: 0;
		display: block;
	}

	.welcome-description {
		text-align: center;
		font-size: 15px;
		font-family: var(--font-bold);
	}
	.hashtag {
		margin-bottom: 15px;
		text-align: center;
	}
</style>
