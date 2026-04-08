<script>
let { initialCount: count = $bindable() } = $props();
let doubled = $derived(count * 2);
</script>

<h3>Clicks Counter</h3>

<button onclick={() => count++}>
    clicks: {count}
</button>

<style>
    h1 {
        color: deepskyblue;
    }
</style>

<span>doubled is {doubled}</span>