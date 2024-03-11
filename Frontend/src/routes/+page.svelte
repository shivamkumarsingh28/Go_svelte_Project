
<script>
    import Card from "../component/card.svelte";
    import Header from "../component/header.svelte";
    import { onMount } from "svelte";
    import Hero from "../component/hero.svelte";
    import Footer from "../component/footer.svelte";
    const endpoint = "https://jsonplaceholder.typicode.com/posts";
    let posts = [];
  
    onMount(async function () {
      const response = await fetch(endpoint);
      const data = await response.json();
      // console.log(data);
      posts = data;
    });
  
  </script>

<svelte:head>
	<link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/css/bootstrap.min.css" rel="stylesheet" integrity="sha384-QWTKZyjpPEjISv5WaRU9OFeRpok6YctnYmDr5pNlyT2bRjXh0JMhjY6hW+ALEwIH" crossorigin="anonymous">
</svelte:head>
  

  <Header />
  <Hero />
  <Card />
 <!-- <Cart /> -->
  <Footer />

  <style>
    /* ommitted for brevity */
  </style>
