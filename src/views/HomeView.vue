<template>
  <section class="sticky-area">
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
            <li class="nav-item">
              <a class="nav-link" href="#sobre">Sobre mim</a>
            </li>
            <li class="nav-item">
              <a class="nav-link" href="#conhecimentos">Conhecimentos</a>
            </li>
            <li class="nav-item">
              <a class="nav-link" href="#portifolio">Portifolio</a>
            </li>
            <li class="nav-item">
              <a class="nav-link" href="https://paulodev367.com.br/">Blog</a>
            </li>
          </ul>
        </div>
      </div>
    </nav>
  </section>

  <div class="conteudo-principal">
    <header>
      <div class="container">
        <div class="row align-items-center flex-wrap-reverse">
          <div class="col-12 col-md-6">
            <h2>Olá</h2>
            <h1>Eu sou Paulo Silva</h1>
            <h3>Desenvolvedor Fullstack</h3>
            <ul>
              <li>
                <a href="https://github.com/PauloDev367" title="Meu Github">
                  <i class="fa-brands fa-github"></i>
                </a>
              </li>
              <li>
                <a href="https://www.linkedin.com/in/paulo-henrique-almeida-silva-9234171b3/" title="Meu Linkedin">
                  <i class="fa-brands fa-linkedin"></i>
                </a>
              </li>
              <li>
                <a href="https://paulodev367.com.br/" title="Meu Blog">
                  <i class="fa-regular fa-newspaper"></i>
                </a>
              </li>
            </ul>
            <a href="#portifolio">Ver projetos</a>
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
          <div class="col-12 col-lg-6">
            <img src="../assets/images/2.jpg" alt="Complementar" class="w-100">
          </div>
          <div class="col-12 col-lg-6">
            <h2>Deixe-me apresentar</h2>
            <p>
              Olá, sou Paulo Silva, um entusiasta da tecnologia e, atualmente, Desenvolvedor de Software na Luma
              Digital. Minha paixão por codificação se reflete em minha proficiência em diversas linguagens e
              tecnologias,
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

    <section id="blog">
      <div class="cotainer">
        <div class="row">
          <div class="col-12">
            <h2>Não deixe de visitar meu blog</h2>
            <p>
              Nele posto semanalmente artigos com dicas de tecnologias utilizadas no mercado de
              desenvolvimento. Sempre tentando trazer algo a mais para que você possa aumentar seus
              conhecimentos
            </p>
            <div class="cta">
              <a href="https://paulodev367.com.br/" target="_blank">
                Acesse agora
              </a>
            </div>
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
            <a href="/pdf/projetos/9.pdf" download="9.pdf" class="card-portifolio">
              <img src="../assets/images/projetos/1.png" class="w-100" alt="Projeto Feedbacks">
            </a>
          </div>
          <div class="col-6 col-md-4">
            <a href="/pdf/projetos/8.pdf" download="1.pdf" class="card-portifolio">
              <img src="../assets/images/projetos/2.png" class="w-100" alt="Projeto PIX Mercado Pago">
            </a>
          </div>
          <div class="col-6 col-md-4">
            <a href="/pdf/projetos/7.pdf" download="1.pdf" class="card-portifolio">
              <img src="../assets/images/projetos/3.png" class="w-100" alt="Projeto Busshopping">
            </a>
          </div>
          <div class="col-6 col-md-4">
            <a href="/pdf/projetos/6.pdf" download="6.pdf" class="card-portifolio">
              <img src="../assets/images/projetos/4.png" class="w-100" alt="Projeto IBM + CF2Forum">
            </a>
          </div>
          <div class="col-6 col-md-4">
            <a href="/pdf/projetos/5.pdf" download="5.pdf" class="card-portifolio">
              <img src="../assets/images/projetos/5.png" class="w-100" alt="Projeto Pipefy">
            </a>
          </div>
          <div class="col-6 col-md-4">
            <a href="/pdf/projetos/4.pdf" download="4.pdf" class="card-portifolio">
              <img src="../assets/images/projetos/6.png" class="w-100" alt="Projeto Mini Portal">
            </a>
          </div>
          <div class="col-6 col-md-4">
            <a href="/pdf/projetos/3.pdf" download="3.pdf" class="card-portifolio">
              <img src="../assets/images/projetos/7.png" class="w-100" alt="Projeto Transfer do Torcedor">
            </a>
          </div>
          <div class="col-6 col-md-4">
            <a href="/pdf/projetos/2.pdf" download="2.pdf" class="card-portifolio">
              <img src="../assets/images/projetos/8.png" class="w-100" alt="Projeto Controle de Estoque">
            </a>
          </div>
          <div class="col-6 col-md-4">
            <a href="/pdf/projetos/1.pdf" download="1.pdf" class="card-portifolio">
              <img src="../assets/images/projetos/9.png" class="w-100" alt="Projeto Ingressos Online">
            </a>
          </div>

        </div>
      </div>
    </section>

    <section id="casos">
      <div class="container">
        <div class="row align-items-center">
          <div class="col-12">
            <h2>MAIS DO QUE O ESPERADO</h2>
          </div>
          <div class="col-12 col-lg-6">
            <p>
              Além de possuir os conhecimentos necessários para desenvolver projetos de alta qualidade por meio de
              código, tenho experiência prática nas etapas fundamentais da engenharia de software. Já participei das
              seguintes etapas:
            </p>
            <ul>
              <li>Levantamento de requisitos</li>
              <li>Elaboração de diagramas de casos de uso</li>
              <li>Elaboração de diagramas de classe</li>
              <li>Criação de wireframes em ferramentas como Figma</li>
              <li>Criação de layouts completos no Figma</li>
              <li>Atendimento ao cliente pós-desenvolvimento</li>
              <li>Treinamento de uso da plataforma</li>
            </ul>
            <p>
              Essa combinação de habilidades técnicas e experiência prática permite-me contribuir significativamente
              para o sucesso de qualquer projeto.

            </p>
          </div>
          <div class="col-12 col-md-6">
            <div id="carouselDiagram" class="carousel slide" data-ride="carousel">
              <div class="carousel-inner">
                <div class="carousel-item active">
                  <img class="d-block w-100" src="../assets/images/diagramas/1.png" alt="First slide">
                </div>
                <div class="carousel-item">
                  <img class="d-block w-100" src="../assets/images/diagramas/2.jpeg" alt="Second slide">
                </div>
                <div class="carousel-item">
                  <img class="d-block w-100" src="../assets/images/diagramas/3.jpeg" alt="Third slide">
                </div>
                <div class="carousel-item">
                  <img class="d-block w-100" src="../assets/images/diagramas/4.jpeg" alt="Second slide">
                </div>
                <div class="carousel-item">
                  <img class="d-block w-100" src="../assets/images/diagramas/5.jpeg" alt="Third slide">
                </div>
              </div>
              <a class="carousel-control-prev" href="#carouselDiagram" role="button" data-slide="prev">
                <span class="carousel-control-prev-icon" aria-hidden="true"></span>
                <span class="sr-only">Previous</span>
              </a>
              <a class="carousel-control-next" href="#carouselDiagram" role="button" data-slide="next">
                <span class="carousel-control-next-icon" aria-hidden="true"></span>
                <span class="sr-only">Next</span>
              </a>
            </div>
          </div>
        </div>
      </div>
    </section>

    <footer class="bg-dark">
      <ul>
        <li>
          <a href="https://github.com/PauloDev367" title="Meu Github">
            <i class="fa-brands fa-github"></i>
          </a>
        </li>
        <li>
          <a href="https://www.linkedin.com/in/paulo-henrique-almeida-silva-9234171b3/" title="Meu Linkedin">
            <i class="fa-brands fa-linkedin"></i>
          </a>
        </li>
        <li>
          <a href="https://paulodev367.com.br/" title="Meu Blog">
            <i class="fa-regular fa-newspaper"></i>
          </a>
        </li>
      </ul>
    </footer>
  </div>
</template>

<script>
import "./../assets/css/custom.css";
export default {
  name: 'HomeView',
}
</script>