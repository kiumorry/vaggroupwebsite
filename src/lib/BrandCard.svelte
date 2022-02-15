<script>
	export let brand;
</script>

<a href="/brands/{brand.id}">
	<div class="p-4 rounded-lg border-2 border-gray-200 hover:bg-gray-100">
		<div>
			<img class="w-full" src="{brand.images.logo}" alt="Логотип {brand.name}">
		</div>
		<h3 class="mt-2 text-2xl font-medium font-roboto text-center">{brand.name}</h3>
	</div>
</a>