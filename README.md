# Ecos-do-veu
<!DOCTYPE html><html lang="pt-br">
<head>
  <meta charset="UTF-8">
  <title>Ecos do Véu</title>
  <style>
    body {
      background-color: #0a0a0a;
      color: #e60000;
      font-family: "Courier New", monospace;
      margin: 0;
      padding: 0;
    }header {
  text-align: center;
  padding: 40px;
  border-bottom: 1px solid #e60000;
}

h1 {
  font-size: 40px;
  letter-spacing: 3px;
}

.container {
  padding: 20px;
}

.card {
  border: 1px solid #e60000;
  padding: 15px;
  margin: 10px 0;
  cursor: pointer;
  transition: 0.3s;
}

.card:hover {
  background-color: #1a0000;
}

.hidden {
  display: none;
  margin-top: 10px;
  color: #ffffff;
}

.glitch {
  animation: glitch 1s infinite;
}

@keyframes glitch {
  0% { text-shadow: 2px 0 red; }
  25% { text-shadow: -2px 0 blue; }
  50% { text-shadow: 2px 0 red; }
  75% { text-shadow: -2px 0 blue; }
  100% { text-shadow: 2px 0 red; }
}

.secret {
  position: fixed;
  bottom: 10px;
  right: 10px;
  font-size: 10px;
  color: #222;
}

.secret:hover {
  color: red;
}

  </style>
</head>
<body><header>
  <h1 class="glitch">ECOS DO VÉU</h1>
  <p>O registro está aberto.</p>
</header><div class="container">  <div class="card" onclick="toggle('arquivo1')">
    📁 Arquivo 001 - Entidade: El Cuco
    <div id="arquivo1" class="hidden">
      Uma presença que observa crianças durante o sono. Não confie nos reflexos.
    </div>
  </div>  <div class="card" onclick="toggle('arquivo2')">
    📁 Arquivo 002 - Encapuzados Vermelhos
    <div id="arquivo2" class="hidden">
      Eles mantêm o equilíbrio do Véu. Mas a que custo?
    </div>
  </div>  <div class="card" onclick="toggle('arquivo3')">
    📁 Arquivo 003 - Relíquia: Capuz Rubro
    <div id="arquivo3" class="hidden">
      Aquele que veste o capuz nunca mais dorme em paz.
    </div>
  </div></div><div class="secret" onclick="senha()">...</div><script>
  function toggle(id) {
    var el = document.getElementById(id);
    el.style.display = el.style.display === "block" ? "none" : "block";
  }

  function senha() {
    var resposta = prompt("Digite a senha:");
    if(resposta === "7") {
      alert("Você foi marcado pelo Véu.");
    } else {
      alert("Acesso negado.");
    }
  }
</script></body>
</html>
