<script>
    import Cart from "./Cart/cart.svelte";
    // import Card from "./card.svelte";

</script>
<div class="position-relative overflow-hidden p-3 p-md-5 m-md-3 text-center bg-body-tertiary">
    <div class="col-md-6 p-lg-5 mx-auto my-5">
      <h1 class="display-3 fw-bold">Product Card Show Here</h1>
      <!-- <h3 class="fw-normal text-muted mb-3">Build anything you want with Aperture</h3> -->
      <div class="d-flex gap-3 justify-content-center lead fw-normal">
        <Cart />
      </div>
    </div>
    <div class="product-device shadow-sm d-none d-md-block"></div>
    <div class="product-device product-device-2 shadow-sm d-none d-md-block"></div>
  </div>