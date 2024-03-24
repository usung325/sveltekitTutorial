<script>
    let quantity = 0;

    function addToCart() {
        quantity = quantity + 1;
        // inventory.push(quantity);
        // inventory = inventory;
        inventory = [...inventory, quantity];
    };

    let inventory = [1, 2, 3];
    //reactive statement
    $: remain = 10 - quantity;

    let price = 5;
    $: reactivePrice = price + quantity;
    $: if (quantity === 10) {
        alert(`lmao ${quantity}`);
    }
</script>


<p class="m-4">hello my name is {quantity}</p>

<button on:click={addToCart} class="m-4 p-2 bg-blue-500 rounded-md text-white">button</button>
<p>{inventory}</p>
<p> {remain} button clicks left</p>
<p>{reactivePrice}</p>