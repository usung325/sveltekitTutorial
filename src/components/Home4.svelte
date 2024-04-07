<script>
    let product = {
        name: 't-shirt',
        quantity: 0
    };

    function increment(){
        product.quantity += 1;
    }
</script>
<div class="p-10">
    {#if product.quantity >= 10}
    <div class="bg-green-300">
        this product is in stock
    </div>
        {:else if product.quantity == 0}
        <div class="bg-yellow-300">
            this product is not in stock
        </div>
        {:else}
        <div class="bg-red-300">
            not enough quantity to ship
        </div>
    {/if}
    <div>
        <h3>
            Current {product.name} Quantity: {product.quantity}
        </h3>
    </div>

    <div>
        <button class="outline outline-1" on:click={()=>{increment()}}> add {product.name} to inventory </button>
    </div>
</div>

