<script>
	import { onMount } from 'svelte';

	import Swiper, { Navigation } from 'swiper';
	import 'swiper/css';
	import 'swiper/css/navigation';
	
	onMount(() => {
		const swiper = new Swiper(".swiper", {
			modules: [Navigation],
			slidesPerView: 4,
			spaceBetween: 30,
			navigation: {
				nextEl: '.swiper-button-next',
				prevEl: '.swiper-button-prev',
			},
		});
	});
</script>

<div class="container py-8 md:px-32 px-8">
	<h1 class="text-4xl font-medium font-roboto">Volkswagen Group</h1>
	
	<p class="mt-8 text-xl font-montserrat">
		<b>Volkswagen AG</b>, известный на международном уровне как <b>Volkswagen Group</b>,
		является немецким многонациональным производителем автомобилей
		со штаб-квартирой в Вольфсбурге, Нижняя Саксония, Германия.
		<b>Volkswagen Group</b> продает такие автомобили как:
		Volkswagen, Audi, Bentley, Bugatti, Lamborghini, Porsche,
		SEAT, Skoda, Man, Scania, а так же мотоциклы Ducati.
	</p>

	<div class="flex flex-col items-center">
		<img class="mt-8 mx-auto w-6/12 rounded-lg" src="/images/VW.jpg" alt="Здание Volkswagen">
		<p class="mt-2 text-gray-500 text-sm">Завод <b>Volkswagen AG</b></p>
	</div>

	<p class="mt-16 text-xl font-montserrat">
		Модельный ряд концерна охватывает широкий спектр транспортных
		средств от мотоциклов и экономичных малолитражных автомобилей
		до автомобилей класса люкс. В сегменте коммерческих автомобилей
		представлены различные варианты от пикапов до автобусов и тяжелых
		грузовых автомобилей.
	</p>

	<div class="mt-16 swiper">
		<div class="swiper-wrapper">
			<div class="swiper-slide">
				<img class="select-none" src="/images/logos/vw-logo.png" alt="">
			</div>
			<div class="swiper-slide">
				<img class="select-none" src="/images/logos/skoda-logo.png" alt="">
			</div>
			<div class="swiper-slide">
				<img class="select-none" src="/images/logos/audi-logo.png" alt="">
			</div>
			<div class="swiper-slide">
				<img class="select-none" src="/images/logos/porsche-logo.png" alt="">
			</div>
			<div class="swiper-slide">
				<img class="select-none" src="/images/logos/lamborghini-logo.png" alt="">
			</div>
			<div class="swiper-slide">
				<img class="select-none" src="/images/logos/bentley-logo.png" alt="">
			</div>
		</div>

		<div class="swiper-button-prev"></div>
		<div class="swiper-button-next"></div>
	</div>

	<p class="mt-16 text-xl font-montserrat">
		Концерн Volkswagen имеет 
		<span class="text-2xl font-bold text-orange-500">118</span>
		заводов в <span class="text-2xl font-bold text-red-500">20</span> 
		странах Европы и 
		<span class="text-2xl font-bold text-purple-500">10</span>
		странах Северной и Южной Америки, Азии и Африки. Каждый будний день 
		<span class="text-2xl font-bold text-yellow-500">662 575</span>
		сотрудника концерна по всему миру производят около 
		<span class="text-2xl font-bold text-cyan-500">34 900</span>
		автомобилей и работают в других сферах бизнеса. Volkswagen Group
		продает свои автомобили в 
		<span class="text-2xl font-bold text-blue-500">153</span> 
		странах мира.
	</p>

	<div class="my-16 flex flex-col items-center">
		<iframe src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d155780.32225172277!2d10.636477196305018!3d52.405452217585086!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x47af92424757e6b1%3A0x425ac6d94ac3ad0!2sWolfsburg%2C%20Germany!5e0!3m2!1sen!2sru!4v1644880987737!5m2!1sen!2sru" width="100%" height="400" style="border:0;" allowfullscreen="" loading="lazy" title="Штаб квартира Volkswagen Group"></iframe>
		<p class="mt-2 text-gray-500 text-sm">Штаб квартира <b>Volkswagen AG</b></p>
	</div>
</div>

