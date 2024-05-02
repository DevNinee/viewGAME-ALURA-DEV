# viewGAME-ALURA-DEV

HTML

<html>

<head>
  <title>
    Imersão Dev - Aula 05
  </title>
</head>

<body>
  <div class="container">
    <h1 class="page-title">
      ViewGAME
    </h1>
    <img src="" alt="">
    <p class="page-subtitle">
      Quais são seus jogos favoritos ?
    </p>
    <div class="form-wrapper">
      <input type="text" id="jogo" name="jogo" placeholder="Insira endereço de imagem">
      <button onClick="adicionar jogo()">adicionar jogo</button>
    </div>
  </div>
  <div id="adicionarjogo"></div>
  <a href="" target="_blank">
    <img src="">
  </a>
</body>

</html>

CSS

body {
  font-family: "Roboto Mono", monospace;
  text-align: center;
  background-image: url("");
  background-color: black;
  background-size: cover;
  background-position: center top;
  background-repeat: no-repeat;
}

.container {
  text-align: center;
  padding: 20px;
}

.page-title {
  color: #ffffff;
  margin: 0 0 5px;
}

.page-subtitle {
  color: green;
  margin-top: 5px;
  font-family: "cursive";
}

.page-logo {
  width: 200px;
}

.alura-logo {
  width: 40px;
  position: absolute;
  top: 10px;
  right: 10px;
}

#listajogos img {
  margin: 10px;
  max-height: 250px;
}

.form-wrapper {
  margin: 0 0 15px;
}

.form-wrapper input {
  display: block;
  margin: 0 auto;
  padding: 10px 15px;
}

.form-wrapper button {
  border: 0;
  color: #ffffff;
  background: #da1e26;
  font-weight: bold;
  padding: 15px 20px;
  font-size: 16px;
  border-radius: 4px;
  margin-top: 20px;
  cursor: pointer;
  transition: 0.3s;
}

.form-wrapper button:hover {
  opacity: 0.8;
}

JAVASCRPIT


function adicionarjogo() {
  var jogoFavorito = document.getElementById("Jogo").value;
  if (jogoFavorito.endsWith(".jpg")) {
    var elementoJogofavorito = "<img src=" + JogoFavorito + ">";
    var elementoListaJogos = document.getElementById("listaJogos");
    elementoListaJogos.innerHTML =
      elementoListaJogos.innerHTML + elementoJogofavorito;
}


