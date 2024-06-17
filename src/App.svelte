<script lang="ts">
    import HomePage from './lib/HomePage.svelte';
  import Tables from './lib/HomePage.svelte'
  import Router from 'svelte-spa-router'

  const routes = {
    // Exact path
    '/': HomePage,
    //'/orders': Orders,

    // Using named parameters, with last being optional
    //'/table/:id/': Table,
    // TO GET TO THE ID: export let params: any = {}; params.id;


    // Catch-all
    // This is optional, but if present it must be the last
    //'*': NotFound,
  }
</script>

<main>
  <Router {routes}/>
</main>

<style>

</style>