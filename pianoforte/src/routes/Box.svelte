<script>

	/**
	 * @type {{ title: string; author: string; create_date: Date; body: string; }}
	 */
	 export let item;
</script>

<div class="prose prose-slate">
	<slot><h2 class="">{ item.title }</h2></slot>
	<hr>
	<slot><h3 class="">by: { item.author }</h3></slot>
	<slot><p class="">on: { item.create_date.toLocaleDateString() }</p></slot>
	<hr>
	<slot>{ item.body }</slot>
</div>
