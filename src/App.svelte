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