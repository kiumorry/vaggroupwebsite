<script context="module">
	import vag from "../../vag.json";

	export async function load(ctx) {
		return {
			props: {
				brand: vag[ctx.params.id - 1],
			},
		}
	}
</script>

<script>
	export let brand;
</script>


<img class="w-full mb-8" src="{brand.images.promo}" alt="Промо {brand.name}">

<div class="container py-8 mb-8 md:px-32 px-8">
	<h1 class="text-4xl font-medium font-roboto">{brand.name}</h1>
	<p class="mb-8 text-gray-600 ">Основан в {brand.date} году {brand.creator}</p>

	<p class="text-xl mb-8 font-montserrat">{brand.description[0]}</p>
	<p class="text-xl mb-8 font-montserrat">{brand.description[1]}</p>

	<p class="text-xl font-montserrat">
		Популярные модели: {brand.popular} 
	</p>
</div>