<h1>Carousel A</h1>
<Carousel>
  <div class="isi a">1</div>
  <div class="isi b">2</div>
  <div class="isi c">3</div>
  <div class="isi d">4</div>
  <div class="isi e">5</div>
</Carousel>
<h1>Carousel B</h1>
<Carousel>
  {#each kode as item, index}
    <div class="full"><img src="https://http.cat/{item}" alt=""></div>
  {/each}
</Carousel>

<script>
  import Carousel from '/src/lib/Carousel.svelte'
  const kode = [101, 200, 404, 500, 403]
</script>

<style lang="scss">
  .full {
    width: 100%;
    img {
      width: inherit;
    }
  }
  .isi {
    $padding: 30px;
    width: 50%; /* important */
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