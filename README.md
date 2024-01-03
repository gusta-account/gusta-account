<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <title>Pedido de Casamento</title>
</head>
<body>
    <div>
        <h1>Casa comigo?</h1>
        <form action="javascript:void(0);" onsubmit="return responderPedido()">
            <button type="submit">Sim</button>
            <button type="button" onclick="recusarPedido()">Não</button>
        </form>
        <div id="resposta"></div>
    </div>

    <script>
        function responderPedido() {
            var resposta = confirm('Parabéns! Você aceita se casar?');
            if (resposta) {
                window.location.href = 'https://www.youtube.com/watch?v=3v3ZXLDLmIs'; // Link para a música de Beethoven
            } else {
                document.getElementById('resposta').innerHTML = 'Você não tem escolha, ouaceita ou você morre.';
            }
            return false; // Impede o envio do formulário
        }

        function recusarPedido() {
            document.getElementById('resposta').innerHTML = 'Você não tem escolha.';
        }
    </script>
</body>
</html>
