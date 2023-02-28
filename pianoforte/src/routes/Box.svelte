<script>

	/**
	 * @type {{ title: string; author: string; create_date: Date; body: string; }}
	 */
	 export let item;
</script>

<span class="bg-gray-200 p-4">
	<div class="prose">
		<h2 class="text-center text-gray-700 bg-gray-400 py-2">{ item.title }</h2>
		<p class="p-4">{ item.body }</p>
		<p class="text-center text-xs uppercase">by: { item.author } on: { item.create_date.toLocaleDateString() }</p>
	</div>
</span>

<style>
	.prose {
		border: solid 2px;
		border-radius: 5px;
		
	}
</style>