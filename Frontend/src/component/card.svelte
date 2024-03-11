<script>
    import { onMount } from "svelte";
    import { cart } from "./Cart/cartStore";
    const endpoint = "https://fakestoreapi.com/products";
    export let posts = [];
  
    onMount(async function () {
      const response = await fetch(endpoint);
      const data = await response.json();
      posts = data;
    });
  
</script>

<div class="container">
    <div class="card-deck row">


        <div class="row row-cols-1 row-cols-sm-2 row-cols-md-3 g-3">
            {#each posts as post}
            <div class="col">
              <div class="card shadow-sm">
                <img class="bd-placeholder-img card-img-top" width="100%" height="225" src={post.image} />
                <div class="card-body">
                  <p class="card-header">{post.title} </p>

                  <p class="card-text">{post.description}</p>
                  <div class="d-flex justify-content-between align-items-center">
                    <div class="btn-group">
                        <button class="btn btn-success" on:click={() => cart.addItem(post)}>Add to Cart</button>
                    </div>
                    <small class="text-body-secondary">{post.category}</small>
                    <small class="text-body-secondary">{post.price}</small>
                  </div>
                </div>
              </div>
            </div>
            {/each}
          </div>
     
    </div>
</div>
