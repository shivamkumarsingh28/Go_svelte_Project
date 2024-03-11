<!-- src/components/Cart.svelte -->
<script>
    // import { LOGNAME } from '$env/static/private';
    import { cart } from './cartStore.js';
    console.log($cart.items);
  </script>
  
  <section>
    <h2>Shopping Cart</h2>
    <ul>
      {#each $cart.items as item (item.id)}
      
        <li>
          <span>{item.title} - {item.quantity} x ${item.price.toFixed(2)}</span>
          <button class="btn btn-danger" on:click={() => cart.removeItem(item.id)}>Remove</button>
        </li>
      {/each}
    </ul>
    <p>Total: ${$cart.total.toFixed(2)}</p>
    <button class="btn btn-primary" on:click={() => cart.clear}>Clear Cart</button>
  </section>