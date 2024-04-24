<script>
    export let pais;
    let p;
    const paises = {
        colombia: [
            "Colombia",
            "Bogota",
            "51,52 millones",
            "Peso colombiano",
            "1,142 millones km2",
            "Flag_of_Colombia.svg",
        ],
        venezuela: [
            "Venezuela",
            "Caracas",
            "28,2 millones",
            "Bolivar",
            " 916.445 km2",
            "Flag_of_Venezuela.svg",
        ],
        ecuador: [
            "Ecuador",
            "Quito",
            "17,8 millones",
            "Dólar estadounidense",
            "256.370 km2",
            "Flag_of_Ecuador.svg",
        ],
        peru: [
            "Peru",
            "Lima",
            "33,72 millones",
            "Sol peruano",
            "1.285.215 km2",
            "800px-Flag_of_Peru_(state).svg.webp",
        ],
        brasil: [
            "Brasil",
            "Brasilia",
            "214,3 millones",
            "Real brasileño",
            "8,51 millones km2",
            "Flag_of_Brazil.svg",
        ],
    };
    p = paises[pais];
</script>

<div class="main">
    <div class="col1">
        <img
            src="./src/assets/{p[5]}"
            alt="Bandera_colombia"
            width="300"
            height="200"
        />
    </div>
    <div class="col2">
        <div class="linea"><strong>pais</strong> {p[0]}</div>
        <div class="linea"><strong>Capital</strong> {p[1]}</div>
        <div class="linea"><strong>Poblacion</strong> {p[2]}</div>
        <div class="linea"><strong>Moneda</strong> {p[3]}</div>
        <div class="linea"><strong>Extencion</strong> {p[4]}</div>
    </div>
</div>

<style>
    .main {
        display: grid;
        grid-template-columns: repeat (4, 1fr);
        grid-gap: 5px;
        grid-auto-rows: minmax (100px, auto);
        border-radius: 10px;
        border-style: solid;
        border-color: rgb(186, 190, 182);
        border-width: 2px;
        margin: left;
        width: 600px;
        box-shadow: 5px 5px 5px black;
        margin-right: 5px;
        margin-bottom: 10px;
    }
    .col1 {
        grid-column: 1;
        grid-row: 1;
        margin: 5px;
        padding: 5px;
    }
    .co12 {
        grid-column: 2;
        grid-row: 1;
        margin: 5px;
        padding: 5px;
        border-color: black;
        width: max-content;
    }

    strong {
        color: blue;
        font-weight: bolder;
    }
    .linea {
        font-size: 20px;
        margin-bottom: 18px;
    }
</style>
