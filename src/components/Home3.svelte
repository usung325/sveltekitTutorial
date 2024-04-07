<script>
    let searchedVal = '';

    let checked = false;    


</script>

<div class='p-10'>
    <h3>
        Searched: {searchedVal}
    </h3>
    <input class="outline outline-1" bind:value={searchedVal} >

    <br>
    <br>
    
    <h3>
        Checked: {checked}
    </h3>
    <input type="checkbox" bind:checked = {checked} >
</div>

