<!-- Flickity HTML init -->
<div bind:this={elFlickity}>
	<slot></slot>
</div>

<script>
	let elFlickity
	import {onMount} from 'svelte'
	function panggilFlickity(){
		new Flickity(elFlickity, {
			cellAlign: 'left',
			contain: true
		})
	}
	onMount(() => panggilFlickity())
</script>