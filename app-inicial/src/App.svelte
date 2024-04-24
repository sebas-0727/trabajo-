<script>
    import Parimpar from "./lib/parimpar.svelte";
    let valor = 0;
    const listeninput = (event) => (valor = event.target.value);
</script>

<main>
    <Parimpar numero={valor} />
    <input value={valor} on:input={listeninput} />
</main>
