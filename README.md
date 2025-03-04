# Trabalho-Mobile
trabalho do Matheus, programação mobile
<!DOCTYPE html>
<html lang="pt-br">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <style>
        body {
            font-family: Arial, Helvetica, sans-serif;
            background: linear-gradient(to right, #800080, #0000ff);
            height: 100vh;
            margin: 0;
        }

        input {
            padding: 5px;
            border: none;
            font-size: 25px;
            border-radius: 50px;
        }

        button {
            padding: 5%;
            border-radius: 30px;
            font-size: 130%;
            font-family: sans-serif;
            color: aliceblue;
            background-color: #00071f;
            width: 100%;
        }

        form {
            background-color: rgba(0, 14, 78, 0.7);
            position: absolute;
            top: 50%;
            left: 50%;
            transform: translate(-50%, -50%);
            padding: 50px;
            border-radius: 15%;
            color: aliceblue
        }

        h3 {
            font-size: 250%;
        }
    </style>
</head>

<body>
    <form>
        <h3>cadastro</h3>
        <input type="text" id="nome" placeholder="nome">
        <br><br>
        <input type="password" id="senha" placeholder="senha">
        <br><br>
        <input type="text" id="email" placeholder="email">
        <br><br>
        <input type="tel" id="telefone" placeholder="telefone">
        <br><br>
        <button type="button" onclick="logar()"> enviar</button>
    </form>

    <script>
        function logar() {
            var nome = document.getElementById("nome").value
            var senha = document.getElementById("senha").value
            var email = document.getElementById("email").value
            var telefone = document.getElementById("telefone").value
            if (nome === "giovanna" && senha === "123" && email === "giovanna.example.com" && telefone === "123456789") {
                alert("sucesso!!")
                window.location.href = "home.html"
            } else { alert("dados incorretos") }
        }

    </script>
</body>

</html>
