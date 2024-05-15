<template>
  <nav class="navbar navbar-expand-lg navbar-light bg-light">
    <div class="container">
      <a class="navbar-brand" href="/">
        <img alt="Logo" src="../assets/images/logo.png">

      </a>
      <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarSupportedContent"
        aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
        <span class="navbar-toggler-icon"></span>
      </button>

      <div class="collapse navbar-collapse" id="navbarSupportedContent">
        <ul class="navbar-nav ml-auto">
          <li class="nav-item active">
            <a class="nav-link" href="https://paulodev367.com.br/">Meu blog</a>
          </li>
        </ul>
      </div>
    </div>
  </nav>

  <header>
    <div class="container">
      <div class="row align-items-center">
        <div class="col-12 col-md-6">
          <h2>Olá</h2>
          <h1>Eu sou Paulo Silva</h1>
          <h3>Desenvolvedor Fullstack</h3>
          <a href="#">Ver projetos</a>
        </div>
        <div class="col-12 col-md-6">
          <img alt="Header" src="../assets/images/home-right.png" class="w-100">
        </div>
      </div>
    </div>
  </header>

  <section id="sobre">
    <div class="container">
      <div class="row align-items-center">
        <div class="col-12 col-md-6">
          <img src="../assets/images/2.jpg" alt="Complementar" class="w-100">
        </div>
        <div class="col-12 col-md-6">
          <h2>Deixe-me apresentar</h2>
          <p>
            Olá, sou Paulo Silva, um entusiasta da tecnologia e, atualmente, Desenvolvedor de Software na Luma
            Digital. Minha paixão por codificação se reflete em minha proficiência em diversas linguagens e tecnologias,
            como PHP, C#, JavaScript, entre outras.
          </p>
          <p>
            Além disso, como um bom profissional, possuo também
            habilidades linguisticas podendo me comunicar em português nativo e inglês intermediario,
            o que me permite colaborar com toda minha equipe da melhor forma possível.
          </p>
          <p>
            Sou uma pessoa autodidata, sempre buscando novos conhecimentos e ferramentas que possam
            me ajudar no meu dia a dia, seja de forma técnica, ou até mesmo metodologias que melhorem o
            fluxo e organização do meu trabalho.
          </p>
          <a href="#">Baixar currículo</a>
        </div>
      </div>
    </div>
  </section>

  <section id="conhecimentos">
    <div class="container">
      <div class="row">
        <div class="col-12 text-center">
          <h2>Conhecimentos</h2>
          <p>
            Com mais de 3 anos de experiência, trago comigo um bom conjunto de tecnologias as quais já trabalhei
            e julgo importante para desenvolver soluções da melhor forma possível
          </p>
        </div>
        <div class="col-12">
          <div id="carouselConhe" class="carousel slide" data-ride="carousel">
            <div class="carousel-inner">

              <div class="carousel-item active">
                <div class="row">
                  <div class="col-6 col-md-3">
                    <img src="../assets/images/conhecimentos/1.png" class="d-block w-100" alt="Tecnologia">
                  </div>
                  <div class="col-6 col-md-3">
                    <img src="../assets/images/conhecimentos/2.png" class="d-block w-100" alt="Tecnologia">
                  </div>
                  <div class="col-6 col-md-3">
                    <img src="../assets/images/conhecimentos/3.png" class="d-block w-100" alt="Tecnologia">
                  </div>
                  <div class="col-6 col-md-3">
                    <img src="../assets/images/conhecimentos/4.png" class="d-block w-100" alt="Tecnologia">
                  </div>
                </div>
              </div>

              <div class="carousel-item">
                <div class="row">
                  <div class="col-6 col-md-3">
                    <img src="../assets/images/conhecimentos/5.png" class="d-block w-100" alt="Tecnologia">
                  </div>
                  <div class="col-6 col-md-3">
                    <img src="../assets/images/conhecimentos/6.png" class="d-block w-100" alt="Tecnologia">
                  </div>
                  <div class="col-6 col-md-3">
                    <img src="../assets/images/conhecimentos/7.png" class="d-block w-100" alt="Tecnologia">
                  </div>
                  <div class="col-6 col-md-3">
                    <img src="../assets/images/conhecimentos/8.png" class="d-block w-100" alt="Tecnologia">
                  </div>
                </div>
              </div>

              <div class="carousel-item">
                <div class="row">
                  <div class="col-6 col-md-3">
                    <img src="../assets/images/conhecimentos/9.png" class="d-block w-100" alt="Tecnologia">
                  </div>
                  <div class="col-6 col-md-3">
                    <img src="../assets/images/conhecimentos/10.png" class="d-block w-100" alt="Tecnologia">
                  </div>
                  <div class="col-6 col-md-3">
                    <img src="../assets/images/conhecimentos/11.png" class="d-block w-100" alt="Tecnologia">
                  </div>
                  <div class="col-6 col-md-3">
                    <img src="../assets/images/conhecimentos/12.png" class="d-block w-100" alt="Tecnologia">
                  </div>
                </div>
              </div>

              <div class="carousel-item">
                <div class="row">
                  <div class="col-6 col-md-3">
                    <img src="../assets/images/conhecimentos/13.png" class="d-block w-100" alt="Tecnologia">
                  </div>
                  <div class="col-6 col-md-3">
                    <img src="../assets/images/conhecimentos/14.png" class="d-block w-100" alt="Tecnologia">
                  </div>
                  <div class="col-6 col-md-3">
                    <img src="../assets/images/conhecimentos/15.png" class="d-block w-100" alt="Tecnologia">
                  </div>
                </div>
              </div>

            </div>
            <a class="carousel-control-prev" href="#carouselConhe" role="button" data-slide="prev">
              <span class="carousel-control-prev-icon" aria-hidden="true"></span>
              <span class="sr-only">Previous</span>
            </a>
            <a class="carousel-control-next" href="#carouselConhe" role="button" data-slide="next">
              <span class="carousel-control-next-icon" aria-hidden="true"></span>
              <span class="sr-only">Next</span>
            </a>
          </div>
        </div>
      </div>
    </div>
  </section>

  <section id="portifolio">
    <div class="container">
      <div class="row">
        <div class="col-12">
          <h2>Meu portifólio</h2>
          <p>
            Alguns dos projetos desenvolvidos no decorrer da minha carreira. Fique à vontade para navegar
            entre todos eles e baixar o .pdf para visualizar melhor cada um.
          </p>
        </div>

        <div class="col-6 col-md-4">
          <div class="card-portifolio">
            <img src="../assets/images/projetos/1.png" class="w-100" alt="Projeto Feedbacks">
          </div>
        </div>
        <div class="col-6 col-md-4">
          <div class="card-portifolio">
            <img src="../assets/images/projetos/2.png" class="w-100" alt="Projeto PIX Mercado Pago">
          </div>
        </div>
        <div class="col-6 col-md-4">
          <div class="card-portifolio">
            <img src="../assets/images/projetos/3.png" class="w-100" alt="Projeto Busshopping">
          </div>
        </div>
        <div class="col-6 col-md-4">
          <div class="card-portifolio">
            <img src="../assets/images/projetos/4.png" class="w-100" alt="Projeto IBM + CF2Forum">
          </div>
        </div>
        <div class="col-6 col-md-4">
          <div class="card-portifolio">
            <img src="../assets/images/projetos/5.png" class="w-100" alt="Projeto Pipefy">
          </div>
        </div>
        <div class="col-6 col-md-4">
          <div class="card-portifolio">
            <img src="../assets/images/projetos/6.png" class="w-100" alt="Projeto Mini Portal">
          </div>
        </div>
        <div class="col-6 col-md-4">
          <div class="card-portifolio">
            <img src="../assets/images/projetos/7.png" class="w-100" alt="Projeto Transfer do Torcedor">
          </div>
        </div>
        <div class="col-6 col-md-4">
          <div class="card-portifolio">
            <img src="../assets/images/projetos/8.png" class="w-100" alt="Projeto Controle de Estoque">
          </div>
        </div>
        <div class="col-6 col-md-4">
          <div class="card-portifolio">
            <img src="../assets/images/projetos/9.png" class="w-100" alt="Projeto Ingressos Online">
          </div>
        </div>

      </div>
    </div>
  </section>

</template>

<script>

export default {
  name: 'HomeView',
}
</script>

<style>
:root {
  --verde: #70d19e;
}

a:hover {
  text-decoration: none;
}

nav img {
  width: 200px;
}

header {
  padding: 40px 0;
}

header a {
  border: 1px solid var(--verde);
  color: var(--verde);
  display: inline-block;
  padding: 10px 20px;
  transition: all .3s;
  border-radius: 5px;
}

header a:hover {
  background-color: var(--verde);
  color: #fff;
}

#sobre a {
  border: 1px solid var(--verde);
  color: var(--verde);
  display: inline-block;
  padding: 10px 20px;
  transition: all .3s;
  border-radius: 5px;
}

#sobre a:hover {
  background-color: var(--verde);
  color: #fff;
}

#conhecimentos {
  padding: 40px 0;
}

.card-portifolio {
  margin-bottom: 20px;
  border: 2px solid var(--verde);
  transition: all .3s;
  cursor: pointer;
}

.card-portifolio:hover {
  scale: 1.03;
  box-shadow: rgba(0, 0, 0, 0.24) 0px 3px 8px;
}
</style>