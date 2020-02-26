<script>
	let count = 0;

    $: ending = count === 1 ? '' : 's';
    
    function increaseCount() {
        return count++
    }

    export let answer = 'lost in woods', propWithDefault = 'mistery';
</script>

<h1>Hello world!</h1>
<button on:click={increaseCount}>Click to increase the count</button>
<p>Count: {count} time{ending}</p>
<p>Prop passed from the parent is <strong>{answer}</strong></p>
<p>As well we have some prop which's default name is <strong>{propWithDefault}</strong> and it can be overwriten by parent props</p>