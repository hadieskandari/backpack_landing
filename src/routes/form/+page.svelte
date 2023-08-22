<script lang="ts">
	import goodJob from '$lib/images/goodJob.svg';
	import standing from '$lib/images/standing.png';
	import book from '$lib/images/book.png';
	import component from '$lib/images/component.png';
	import hashtag from '$lib/images/hashtag.svg';
</script>

<svelte:head>
	<title>یک کلیک، یک کوله</title>
</svelte:head>

<div class="main-container">
	<div class="text-center">
		<img src={component} alt="backpack" width="310px" height="58px" />
	</div>

	<div class="w-100 text-center mt-1">
		<img src={goodJob} alt="Welcome" width="270px" height="110px" />
	</div>
	<div class="w-100 centralize">
		<div class="text-center">ز طرف تمامی کودکانی که شما بانیِ مهر آن‌ها شدید.</div>
	</div>
	<div class="text-center">
		<img src={standing} alt="Welcome" width="95px" height="235px" />
		<br />
		<img class="image-overlap" src={book} alt="Welcome" width="310px" height="175px" />
	</div>

	<div class="paragraph mt-1">
		<p>
			<strong class="highlight">مهربان پوریا </strong>
			، می‌تونی با زدن دکمه‌ زیر و ذخیره کردن تصویر بالا و منتشر کردن آن به تامین ۱۰،۰۰۰ کوله‌پشتی با
			لوازم التحریر، کمک کنی.
		</p>
	</div>

	<div class="text-center">
		<button>ذخیره کردن</button>
	</div>
</div>

<div class="phone-container">
	<div class="text-center mt-2">
		<span>
			مهربان عزیز، می‌تونید با وارد کردن شماره موبایلتون از مراحل کمپین #مهر_بانی_میخواهد امسال با
			خبر شید.
		</span>
	</div>
	<div class="w-100 mt-2">
		<input type="text" autocomplete="given-name" placeholder="" />
	</div>
	<div class="text-center mt-2">
		<button>ثبت شماره</button>
	</div>
</div>

<div class="message-container">
	<div class="text-center">
		<span>
			اگر دوست دارید، می‌تونید نامه‌ای به کودکی که کوله‌پشتی به دستش می‌رسه، همین پایین بنویسید.
		</span>
	</div>
	<div class="w-100 mt-2">
		<textarea />
	</div>
	<div class="text-center mt-2">
		<button>ارسال نامه</button>
	</div>
</div>

<div class="hashtag mt-2 text-center mb-2">
	<img src={hashtag} alt="hashtag" />
</div>

<style>
	.main-container {
		min-height: 90vh;
		height: 100%;
		background: url('../../lib/images/background.png');
		background-size: cover;
	}
	.message-container {
		min-height: 35vh;
		height: 100%;
		background: url('../../lib/images/RectangleBg.png');
		background-size: cover;
		font-family: var(--font-bold);
		font-size: 18px;
		padding: 40px;
	}
	.centralize {
		width: 100%;
		display: flex;
		justify-content: center;
	}
	.centralize div {
		width: 150px;
		color: #357f80;
		font-family: var(--font-bold);
	}
	.image-overlap {
		margin-top: -10rem;
	}
	.paragraph {
		text-align: center;
		padding: 10px 40px;
		font-family: var(--font-bold);
		font-size: 18px;
	}
	.highlight {
		color: #357f80;
	}

	.phone-container {
		padding: 0 40px;
		margin-bottom: 40px;
	}
	.phone-container span {
		font-family: var(--font-bold);
		font-size: 18px;
	}
</style>
