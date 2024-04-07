<script>
    export let product = {
        name: 'no product',
        price: 0,
        src: '/favicon.png'
    }
    // these are default values above if no props are given
</script>


<div class="p-10 bg-purple-700 flex">
    <div class="my-auto">
        <div class='text-white bg-yellow-400 content-center px-6'>
            {product.name}
        </div>
        <div class="bg-white text-center">
            ${product.price} Mil
        </div>
    </div>
    <div>
        <img alt="The project logo" src={product.src} width=200 />
    </div>
</div>