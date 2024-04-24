<script>
    import paises from "../paises.svelte";
    const lista = ["colombia", "venezuela", "ecuador", "peru", "brasil"];
</script>

<div class="main">
    {#each lista as pais}
        <div>
            <paises{pais} />
        </div>
    {:else}
        no existe elemento
    {/each}
</div>
<svelte:head>
    <title>paises de suramerica</title>
</svelte:head>

<style>
    .main {
        display: grid;
        grid-template-columns: repeat(2, 1fr);
        grid-gap: 10px;
        grid-auto-rows: minmax(100px, auto);
    }
</style>
