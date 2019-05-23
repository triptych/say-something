<script>
    let count = 0;

    function increment() {
        count += 1;
    }

    function decrement(){
        count -= 1;
    }
</script>

{#if count > 10}
    <p>⚠️ That's a little much, don't you think!</p>
{:else if count < -10}
     <p>👻 How low can you go!</p>
{/if}
<div>Count: {count}</div>

<div>Current count: <input bind:value={count} type="number" /></div>


<button on:click={increment}>Increment</button>
<button on:click={decrement}>Decrement</button>