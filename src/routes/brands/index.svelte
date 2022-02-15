<script context="module">
	import vag from "../../vag.json";

	export async function load(ctx) {
		return {
			props: {
				brands: vag,
			}
		}
	}
</script>

<script>
	import BrandCard from "$lib/BrandCard.svelte";

	export let brands;
</script>

<div class="container py-8 mb-8 md:px-32 px-8">
	<h1 class="text-4xl font-medium font-roboto">Бренды Volkswagen Group</h1>
    <div class="mt-8 grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-x-6 gap-y-10 auto-rows-max">
		{#each brands as b}
			<BrandCard brand={b}></BrandCard>
		{/each}
    </div>
</div>
