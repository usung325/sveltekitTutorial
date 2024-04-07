<script>
    import GridTile2 from "../components/GridTile2.svelte";
    import Home from "../components/Home.svelte";
    import Home2 from "../components/Home2.svelte";
    import Home3 from "../components/Home3.svelte";
    import Home4 from "../components/Home4.svelte";
    import Home5 from "../components/Home5.svelte";

    let products = [
        {name: 'Eva01', src:'/images/temp.webp', price: 50},
        {name: 'Eva02', src:'/images/temp2.webp', price: 40},
        {name: 'Eva03', src:'/images/temp3.webp', price: 35}
    ]


</script>

<!-- <Home /> -->
<main class="">
    {#each products as product (product.name)}
        <GridTile2 product = {product} />
    {/each}
    <GridTile2 />
</main>