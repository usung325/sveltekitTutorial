<script>
    let products = [
        {name: 't-shirt', quantity: 10},
        {name: 'mug', quantity: 8},
        {name: 'sticker', quantity: 50},
        {name: 'sweatshirt', quantity: 10}
    ]

    function addProducts(){
        let cup = {name: 'cup', quantity: 5}
        products = [cup, ...products];
    }
    
</script>



<div class="p-10">
    <button class="p-2 outline outline-1" on:click={()=>{addProducts()}}> add cup </button>
    {#each products as product, i (product.name)}  <!-- this is key-ing each blocks -->
        <h3>{product.name}</h3>
        <input type="checkbox">
        <div>{i}</div>
    {/each}
</div>