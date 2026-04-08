<script>
let props = $props(); // gli stiamo dicendo che andremo ad usare props all'intenro del componente
let count = $state(props.initialCount); // gli diciamo prendi initialcount quindi se c'è quello sarà il valore iniziale (se non c'è metti 0)
let doubled = $derived(count * 2);
</script>

<h3>Clicks Counter</h3>

<button onclick={() => count++}>
    Clicks:{count}
</button>

<span> doubled is {doubled}</span>