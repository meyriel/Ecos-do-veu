<!DOCTYPE html>
<html lang="pt-br">
<head>
<meta charset="UTF-8">
<title>Ecos do Véu - Sistema</title>

<style>
body {
  background-color: #0a0a0a;
  color: #e60000;
  font-family: monospace;
  padding: 20px;
}

h1 {
  text-align: center;
}

.container {
  max-width: 800px;
  margin: auto;
}

.box {
  border: 1px solid red;
  padding: 15px;
  margin-bottom: 15px;
}

input {
  width: 100%;
  background: black;
  color: red;
  border: 1px solid red;
  padding: 5px;
}

button {
  background: red;
  color: black;
  border: none;
  padding: 10px;
  cursor: pointer;
}

button:hover {
  background: darkred;
}
</style>
</head>

<body>

<h1>ECOS DO VÉU</h1>

<div class="container">

<div class="box">
<h2>Ficha</h2>

<label>Nome</label>
<input type="text">

<label>Vida</label>
<input type="number" id="vida" value="100">

<label>Sanidade</label>
<input type="number" id="sanidade" value="100">

</div>

<div class="box">
<h2>Atributos</h2>

<label>Força</label>
<input type="number" id="forca" value="1">

<label>Presença</label>
<input type="number" id="presenca" value="1">

</div>

<div class="box">
<h2>Rolagem de Dados</h2>

<button onclick="rolarDado()">Rolar 1d20</button>

<p id="resultado"></p>
</div>

</div>

<script>
function rolarDado() {
  let resultado = Math.floor(Math.random() * 20) + 1;
  document.getElementById("resultado").innerText = "Resultado: " + resultado;
}
</script>

</body>
</html>
