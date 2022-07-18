<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Hi!</title>
    <!-- CSS only -->
<link href="https://cdn.jsdelivr.net/npm/bootstrap@5.2.0-beta1/dist/css/bootstrap.min.css" rel="stylesheet" integrity="sha384-0evHe/X+R7YkIZDRvuzKMRqM+OrBnVFBL6DOitfPri4tjfHxaWutUpFmBp4vmVor" crossorigin="anonymous">
<link rel="stylesheet" href="styles.css">
</head>
<body class="container bg-primary text-white text-center">
    
    <h1 class="bg-indigo-100">¿Quieres ser mi novia?</h1>
    <div class="mt-5">
    <button class="btn btn-light btn-lg" onclick="siquiere()">Si, Acepto</button>
    <button class=" btn btn-danger ms-2 btn-lg" onmouseenter="noquiero(event)">No, ni muerta!</button>
    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.2.0-beta1/dist/js/bootstrap.bundle.min.js"></script>
<script>
function noquiero(evt){
    let target=evt.target;
    let maxWidth=window.innerWidth;
    let maxHeight=window.innerHeight;
    let randonWidth=getRandon(0,maxWidth - target.offsetWidth);
    let randonHeight=getRandon(0,maxHeight - target.offsetHeight);
    target.style.position="absolute";
    target.style.top=randonHeight+'px';
    target.style.left=randonWidth+'px';

}
function siquiere(){
    alert("Felicidades te ganaste el mejor novio del mundo");
}
function getRandon(min, max){
    return Math.floor(Math.random()*(max-min))+min;
}

</script>
</div>
</body>
</html>
