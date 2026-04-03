# Ecos-do-veu
<!DOCTYPE html>
<html lang="pt-br">
<head>
<meta charset="UTF-8">
<title>Ficha RPG</title>
<style>
  body {
    background: #0a0a0a;
    color: #e60000;
    font-family: monospace;
  }
  input {
    background: black;
    color: red;
    border: 1px solid red;
  }
</style>
</head>
<body>

<h1>Ficha de Agente</h1>

Nome: <input id="nome"><br><br>
Força: <input type="number" id="forca"><br><br>

<button onclick="rolar()">Rolar Dado</button>

<p id="resultado"></p>

<script>
function rolar() {
  let valor = Math.floor(Math.random() * 20) + 1;
  document.getElementById("resultado").innerText = "Resultado: " + valor;
}
</script>

</body>
</html>
