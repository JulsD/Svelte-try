<script>
	let count = 0;

    $: ending = count === 1 ? '' : 's';
    
    function increaseCount() {
        return count++
    }
</script>

<h1>Hello world!</h1>
<button on:click={increaseCount}>Click to increase the count</button>
<p>Count: {count} time{ending}</p>