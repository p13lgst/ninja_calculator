<script>
    import { onMount } from 'svelte';
	import { evaluate } from 'mathjs';

    export let displayText;

    let inputElem;

    const lockFocus = () => {
        inputElem.focus();
    }

    onMount(() => {
        inputElem.focus()
    })

    let result = '';

    $: try {
        result = `=${evaluate(displayText) || 0}`;
    } catch (e) {
        result = 'Invalid Expression'
    }

</script>

<style>
    input, input:focus {
        border: none;
        outline: none;
        background: #eee;
        width: 100%;
        font-size: 1.6rem;
        padding: 0.5em;
    }

    span {
        background: #ddd;
        margin-bottom: 0;
        padding: 0.5em;
        display: block;
        font-size: 1.5rem;
        text-align: right;
        width: 100%;
    }
</style>

<input type="text" bind:this={inputElem} on:blur={lockFocus} bind:value={displayText}>
<span>{result}</span>