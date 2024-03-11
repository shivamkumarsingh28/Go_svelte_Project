<script>
  import Search from "./search.svelte";
</script>


<header class="p-3 text-bg-dark">
  <div class="container">
    <div
      class="d-flex flex-wrap align-items-center justify-content-center justify-content-lg-start"
    >
      <a
        href="/"
        class="d-flex align-items-center mb-2 mb-lg-0 text-white text-decoration-none"
      >
        Ecommerce
      </a>

      <ul
        class="nav col-12 col-lg-auto me-lg-auto mb-2 justify-content-center mb-md-0"
      >
   
      </ul>

      <!-- search box -->

        <Search />
      <!-- here -->

      <div class="text-end">
        <a type="button" class="btn btn-outline-light me-2" href="login">Login</a>
        <a type="button" class="btn btn-warning" href="register">Sign-up</a>
      </div>
    </div>
  </div>
</header>
