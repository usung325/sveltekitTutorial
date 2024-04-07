<script>

    function handleClick(string){
        alert(string);
    }
</script>

<button on:click={()=>{handleClick('lol')}}>
    CLick me!
</button>

<div on:mousemove = {()=> {handleClick('say')}} class="bg-green-500 p-10">
    click
    <div class="bg-red-500">
        red
    </div>
</div>