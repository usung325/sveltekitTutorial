<script>
    let quantity = 0;

    function addToCart() {
        quantity = ++quantity
    };
</script>


<p class="m-4">hello my name is {quantity}</p>

<button on:click={addToCart} class="m-4 p-2 bg-blue-500 rounded-md text-white">button</button>