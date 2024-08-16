<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Mostrar Coração</title>
<style>
    body {
        display: flex;
        justify-content: center;
        align-items: center;
        height: 100vh;
        margin: 0;
        background-color: #f0f0f0;
    }

    .coracao {
        display: none;
        font-size: 100px;
        color: red;
        animation: aparecer 1s forwards;
    }

    @keyframes aparecer {
        0% { opacity: 0; transform: scale(0); }
        100% { opacity: 1; transform: scale(1); }
    }
</style>
</head>
<body>

<div class="coracao">&#10084;</div>

<script>
    // Mostra o coração após um pequeno atraso para simular o clique no link
    setTimeout(function() {
        var coracao = document.querySelector('.coracao');
        coracao.style.display = 'block';
    }, 1000); // 1000 milissegundos = 1 segundo
</script>

</body>
