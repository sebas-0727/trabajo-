<script>
    export let numero;
    let resultado;
    $: if (numero === 0) resultado = "neutro";
    else if (numero % 2 === 0) resultado = "par";
    else resultado = "impar";
</script>

<p>el numero {numero} es {resultado}</p>

<style>
    p {
        color: aquamarine;
        font-family: "Segoe UI", Tahoma, Geneva, Verdana, sans-serif;
        font-size: 25px;
    }
</style>
