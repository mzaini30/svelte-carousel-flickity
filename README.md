# Svelte Carousel Flickity

## Install

```bash
npm i -D svelte-carousel-flickity
```

## Pasang di `index.html`

```html
<link rel="stylesheet" href="https://unpkg.com/flickity@2/dist/flickity.min.css">
<script src="https://unpkg.com/flickity@2/dist/flickity.pkgd.min.js"></script>
```

## Menggunakan

```html
<Carousel {isi} {banyak}></Carousel>

<script>
  import Carousel from 'svelte-carousel-flickity'
  const isi = [1, 2, 3, 4, 5]
  const banyak = 2 // artinya, dalam sekali pandang, ada 2 slide yang terlihat
</script>
```

## Repo

https://github.com/mzaini30/svelte-carousel-flickity