<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <link rel="stylesheet" href="estilos.css">
</head>

<body>
    <h1>Ejemplo practico de css grid</h1>
    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Voluptate iste dolore animi unde excepturi, autem
        aliquam minima cumque similique natus. Cum animi commodi blanditiis natus qui repellat, corporis optio incidunt.
    </p>
    <div class="contenedor">
        <div class="intergrid">caja 1</div>
        <div class="intergrid">caja 2</div>
        <div class="intergrid">caja 3</div>
        <div class="intergrid">caja 4</div>
        <div class="intergrid">caja 5</div>
        <div class="intergrid">caja 6</div>
        <div class="intergrid">caja 7</div>
        <div class="intergrid">caja 8</div>
    </div>
</body>

</html>

CSS 

.contenedor{
    display: grid;
    grid-template-columns: repeat(4, 1fr);
    gap: 20px;
    width: 100%;
    max-width: 800px;
}
.intergrid{
    background-color: bisque;
    color: black;
    padding: 40px 20px;
    border-radius: 8px;
    font-size: 1.2rem;
    font-weight: bold;
    text-align: center;
    box-shadow: 0 4px 6px 1px;
    transition: transform 0.3s ease, background-color 0.3s ease
}
.intergrid:hover{
    transform: translateY(-5px);
    background-color: rgb(189, 170, 147);
    cursor: pointer;
}
