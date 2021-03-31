<!-- Flickity HTML init -->
<div class="gallery js-flickity" bind:this={elFlickity}>
	{#each isi as item, index}
  		<div class="gallery-cell" style="width: {100 / banyak}%">{item}</div>
	{/each}
</div>

<script>
	let elFlickity
	export let isi = [1, 2, 3]
	export let banyak = 1
	import {onMount} from 'svelte'
	function panggilFlickity(){
		new Flickity(elFlickity, {
			cellAlign: 'left',
			contain: true
		})
	}
	onMount(() => {
		panggilFlickity()
	})
</script>

<style>
	/* external css: flickity.css */

	* {
	  -webkit-box-sizing: border-box;
	  box-sizing: border-box;
	}

	/*body { font-family: sans-serif; }*/

	.gallery {
	  /*background: #EEE;*/
	}

	.gallery-cell {
	  /*width: 66%;*/
	  /*height: 200px;
	  margin-right: 10px;
	  background: #8C8;*/
	  /*counter-increment: gallery-cell;*/
	}

	/* cell number */
	.gallery-cell:before {
	  /*display: block;
	  text-align: center;*/
	  /*content: counter(gallery-cell);*/
	 /* line-height: 200px;
	  font-size: 80px;
	  color: white;*/
	}
</style>