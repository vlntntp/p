<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Disculpa</title>
    <link rel="stylesheet" href="estilos.css">
</head>
<body>
    <div class="contenedor">
        <p>¿Me disculpas?</p>
        <button id="yesBtn">Sí</button>
        <button id="noBtn">No</Button>
    </div>
    <script src="index.js"></script>
</body>
</html>
*{
    margin: 0;
}

.contenedor{
 background-color: rgb(179, 246, 246);
 width: 100vw;
 height: 100vh;
 text-align: center;
}

p{
    font-size: xx-large;
    padding: 15%;
}

button{
    font-size: xx-large;
    padding: 0.75em;
}

#yesBtn{
    transform: translate(-100%,0);
}

#noBtn{
    position: absolute;
}
		const yesBtn = document.querySelector('#yesBtn');

yesBtn.addEventListener('click',function () {
    alert('Te amo; no me gusta cuando estamos peleados asi')
});

const noBtn = document.querySelector('#noBtn');

noBtn.addEventListener('mouseover',function () {
    const randomX = parseInt(Math.random()*100);
    const randomY = parseInt(Math.random()*100);
    noBtn.style.setProperty('top',randomY+'%');
    noBtn.style.setProperty('left',randomX+'%');
    noBtn.style.setProperty('transform',"translate(-${randomX}%,-${randomY}%)");
});
}
