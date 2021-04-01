# Svelte Carousel Flickity

## Demo

https://svelte-carousel-flickity.vercel.app/

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
<Carousel>
  <div class="isi a">1</div>
  <div class="isi b">2</div>
  <div class="isi c">3</div>
  <div class="isi d">4</div>
  <div class="isi e">5</div>
</Carousel>

<script>
  import Carousel from '/src/lib/Carousel.svelte'
</script>

<style lang="scss">
  .isi {
    $padding: 30px;
    width: 100%; /* important */
    text-align: center;
    padding-top: $padding;
    padding-bottom: $padding;
    &.a {
      background: red;
    }
    &.b {
      background: yellow;
    }
    &.c {
      background: green;
    }
    &.d {
      background: blue;
    }
    &.e {
      background: magenta;
    }
  }
</style>
```

## Repo

https://github.com/mzaini30/svelte-carousel-flickity