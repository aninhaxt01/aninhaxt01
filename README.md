<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" href="styles.css">
    <title>Cartões</title>
</head>
<body>
    <div class="container">
        <div class="card">
            <h2 class="card-title">Pergunta 1</h2>
            <p class="card-text">Esta é a resposta para a pergunta 1.</p>
        </div>
        <div class="card">
            <h2 class="card-title">Pergunta 2</h2>
            <p class="card-text">Esta é a resposta para a pergunta 2.</p>
        </div>
        <div class="card">
            <h2 class="card-title">Pergunta 3</h2>
            <p class="card-text">Esta é a resposta para a pergunta 3.</p>
        </div>
    </div>
</body>
</html>




:root {
    --cor-fundo: #f0f0f0;
    --cor-cartao-fundo: #ffffff;
    --cor-texto: #333333;
    --cor-titulo: #007BFF;
    --imagem-fundo: url('sua-imagem-de-fundo.jpg');
}

body {
    margin: 0;
    padding: 0;
    font-family: Arial, sans-serif;
    background-image: var(--imagem-fundo);
    background-size: cover;
    background-position: center;
}

.container {
    display: flex;
    justify-content: center;
    align-items: flex-start;
    padding: 20px;
    gap: 20px;
}

.card {
    background-color: var(--cor-cartao-fundo);
    color: var(--cor-texto);
    border-radius: 10px;
    box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
    padding: 20px;
    width: 300px; /* Largura fixa dos cartões */
    flex-basis: 30%;
    display: flex;
    flex-direction: column;
    justify-content: space-between;
}

.card-title {
    font-size: 1.5em;
    color: var(--cor-titulo);
    text-align: center;
    margin: 0 0 10px 0;
}

.card-text {
    font-size: 1em;
    line-height: 1.5;
    text-align: justify;
}

/* Responsividade */
@media (max-width: 768px) {
    .container {
        flex-direction: column;
        align-items: center;
    }
}
