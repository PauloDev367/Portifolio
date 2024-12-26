<template>
  <section class="sticky-area">
    <nav class="navbar navbar-expand-lg navbar-light bg-light">
      <div class="container">
        <a class="navbar-brand" href="/">
          <img alt="Logo" src="../assets/images/logo.png" />
        </a>
        <button
          class="navbar-toggler"
          type="button"
          data-toggle="collapse"
          data-target="#navbarSupportedContent"
          aria-controls="navbarSupportedContent"
          aria-expanded="false"
          aria-label="Toggle navigation"
        >
          <span class="navbar-toggler-icon"></span>
        </button>

        <div class="collapse navbar-collapse" id="navbarSupportedContent">
          <ul class="navbar-nav ml-auto">
            <li class="nav-item">
              <a class="nav-link" href="#sobre">About me</a>
            </li>
            <li class="nav-item">
              <a class="nav-link" href="#conhecimentos">Knowledges</a>
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
            <h2>Hello</h2>
            <h1>I am Paulo Silva</h1>
            <h3>Fullstack Developer</h3>
            <ul>
              <li>
                <a href="https://github.com/PauloDev367" title="Meu Github">
                  <i class="fa-brands fa-github"></i>
                </a>
              </li>
              <li>
                <a
                  href="https://www.linkedin.com/in/paulo-henrique-almeida-silva-9234171b3/"
                  title="Meu Linkedin"
                >
                  <i class="fa-brands fa-linkedin"></i>
                </a>
              </li>
              <li>
                <a href="https://paulodev367.com.br/" title="Meu Blog">
                  <i class="fa-regular fa-newspaper"></i>
                </a>
              </li>
            </ul>
            <a href="#portifolio">See my projects</a>
          </div>
          <div class="col-12 col-md-6">
            <img
              alt="Header"
              src="../assets/images/home-right.png"
              class="w-100"
            />
          </div>
        </div>
      </div>
    </header>

    <section id="sobre">
      <div class="container">
        <div class="row align-items-center">
          <div class="col-12 col-lg-6">
            <img
              src="../assets/images/2.jpg"
              alt="Complementar"
              class="w-100"
            />
          </div>
          <div class="col-12 col-lg-6">
            <h2>Let me introduce myself</h2>

            <p>
              Hello, I am Paulo Silva, a technology enthusiast and currently a
              Software Developer at Luma Digital. My passion for coding is
              reflected in my proficiency in various languages and technologies,
              such as PHP, C#, JavaScript, and more.
            </p>
            <p>
              In addition, as a skilled professional, I also have linguistic
              abilities, being able to communicate in native Portuguese and
              intermediate English, which allows me to collaborate effectively
              with my entire team.
            </p>
            <p>
              I am a self-taught person, always seeking new knowledge and tools
              that can help me in my daily work, whether technical or even
              methodologies that improve the flow and organization of my work.
            </p>
          </div>
        </div>
      </div>
    </section>

    <section id="blog">
      <div class="cotainer">
        <div class="row">
          <div class="col-12">
            <h2>Don't forget to visit my blog</h2>
            <p>
              I post weekly articles with tips on technologies used in the
              development market. Always trying to bring something extra so you
              can expand your knowledge.
            </p>
            <div class="cta">
              <a href="https://paulodev367.com.br/" target="_blank">
                Visit now
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
            <h2>Knowledge</h2>
            <p>
              With over 5 years of experience, I bring with me a solid set of
              technologies I have worked with and consider essential for
              developing solutions in the best possible way.
            </p>
          </div>
          <div class="col-12">
            <div id="carouselConhe" class="carousel slide" data-ride="carousel">
              <div class="carousel-inner">
                <div class="carousel-item active">
                  <div class="row">
                    <div class="col-6 col-md-3">
                      <img
                        src="../assets/images/conhecimentos/1.png"
                        class="d-block w-100"
                        alt="Tecnologia"
                      />
                    </div>
                    <div class="col-6 col-md-3">
                      <img
                        src="../assets/images/conhecimentos/2.png"
                        class="d-block w-100"
                        alt="Tecnologia"
                      />
                    </div>
                    <div class="col-6 col-md-3">
                      <img
                        src="../assets/images/conhecimentos/3.png"
                        class="d-block w-100"
                        alt="Tecnologia"
                      />
                    </div>
                    <div class="col-6 col-md-3">
                      <img
                        src="../assets/images/conhecimentos/4.png"
                        class="d-block w-100"
                        alt="Tecnologia"
                      />
                    </div>
                  </div>
                </div>

                <div class="carousel-item">
                  <div class="row">
                    <div class="col-6 col-md-3">
                      <img
                        src="../assets/images/conhecimentos/5.png"
                        class="d-block w-100"
                        alt="Tecnologia"
                      />
                    </div>
                    <div class="col-6 col-md-3">
                      <img
                        src="../assets/images/conhecimentos/6.png"
                        class="d-block w-100"
                        alt="Tecnologia"
                      />
                    </div>
                    <div class="col-6 col-md-3">
                      <img
                        src="../assets/images/conhecimentos/7.png"
                        class="d-block w-100"
                        alt="Tecnologia"
                      />
                    </div>
                    <div class="col-6 col-md-3">
                      <img
                        src="../assets/images/conhecimentos/8.png"
                        class="d-block w-100"
                        alt="Tecnologia"
                      />
                    </div>
                  </div>
                </div>

                <div class="carousel-item">
                  <div class="row">
                    <div class="col-6 col-md-3">
                      <img
                        src="../assets/images/conhecimentos/9.png"
                        class="d-block w-100"
                        alt="Tecnologia"
                      />
                    </div>
                    <div class="col-6 col-md-3">
                      <img
                        src="../assets/images/conhecimentos/10.png"
                        class="d-block w-100"
                        alt="Tecnologia"
                      />
                    </div>
                    <div class="col-6 col-md-3">
                      <img
                        src="../assets/images/conhecimentos/11.png"
                        class="d-block w-100"
                        alt="Tecnologia"
                      />
                    </div>
                    <div class="col-6 col-md-3">
                      <img
                        src="../assets/images/conhecimentos/12.png"
                        class="d-block w-100"
                        alt="Tecnologia"
                      />
                    </div>
                  </div>
                </div>

                <div class="carousel-item">
                  <div class="row">
                    <div class="col-6 col-md-3">
                      <img
                        src="../assets/images/conhecimentos/13.png"
                        class="d-block w-100"
                        alt="Tecnologia"
                      />
                    </div>
                    <div class="col-6 col-md-3">
                      <img
                        src="../assets/images/conhecimentos/14.png"
                        class="d-block w-100"
                        alt="Tecnologia"
                      />
                    </div>
                    <div class="col-6 col-md-3">
                      <img
                        src="../assets/images/conhecimentos/15.png"
                        class="d-block w-100"
                        alt="Tecnologia"
                      />
                    </div>
                    <div class="col-6 col-md-3">
                      <img
                        src="../assets/images/conhecimentos/16.png"
                        class="d-block w-100"
                        alt="Tecnologia"
                      />
                    </div>
                  </div>
                </div>
              </div>
              <a
                class="carousel-control-prev"
                href="#carouselConhe"
                role="button"
                data-slide="prev"
              >
                <span
                  class="carousel-control-prev-icon"
                  aria-hidden="true"
                ></span>
                <span class="sr-only">Previous</span>
              </a>
              <a
                class="carousel-control-next"
                href="#carouselConhe"
                role="button"
                data-slide="next"
              >
                <span
                  class="carousel-control-next-icon"
                  aria-hidden="true"
                ></span>
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
            <h2>My Portfolio</h2>
            <p>
              Some of the projects developed throughout my career. Click to view
              the details of each project.
            </p>
          </div>

          <div class="col-12">
            <ProjetosComponents />
          </div>
        </div>
      </div>
    </section>

    <section id="casos">
      <div class="container">
        <div class="row align-items-center">
          <div class="col-12">
            <h2>MORE THAN EXPECTED</h2>
          </div>
          <div class="col-12 col-lg-6">
            <p>
              In addition to having the necessary knowledge to develop
              high-quality projects through code, I have practical experience in
              the fundamental stages of software engineering. I have been
              involved in the following stages:
            </p>

            <ul>
              <li>Requirements gathering</li>
              <li>Creation of use case diagrams</li>
              <li>Creation of class diagrams</li>
              <li>Creation of wireframes in tools like Figma</li>
              <li>Creation of full layouts in Figma</li>
              <li>Post-development customer support</li>
              <li>Platform usage training</li>
            </ul>
            <p>
              This combination of technical skills and practical experience
              allows me to contribute significantly to the success of any
              project.
            </p>
          </div>
          <div class="col-12 col-md-6">
            <div
              id="carouselDiagram"
              class="carousel slide"
              data-ride="carousel"
            >
              <div class="carousel-inner">
                <div class="carousel-item active">
                  <img
                    class="d-block w-100"
                    src="../assets/images/diagramas/1.png"
                    alt="First slide"
                  />
                </div>
                <div class="carousel-item">
                  <img
                    class="d-block w-100"
                    src="../assets/images/diagramas/2.jpeg"
                    alt="Second slide"
                  />
                </div>
                <div class="carousel-item">
                  <img
                    class="d-block w-100"
                    src="../assets/images/diagramas/3.jpeg"
                    alt="Third slide"
                  />
                </div>
                <div class="carousel-item">
                  <img
                    class="d-block w-100"
                    src="../assets/images/diagramas/4.jpeg"
                    alt="Second slide"
                  />
                </div>
                <div class="carousel-item">
                  <img
                    class="d-block w-100"
                    src="../assets/images/diagramas/5.jpeg"
                    alt="Third slide"
                  />
                </div>
              </div>
              <a
                class="carousel-control-prev"
                href="#carouselDiagram"
                role="button"
                data-slide="prev"
              >
                <span
                  class="carousel-control-prev-icon"
                  aria-hidden="true"
                ></span>
                <span class="sr-only">Previous</span>
              </a>
              <a
                class="carousel-control-next"
                href="#carouselDiagram"
                role="button"
                data-slide="next"
              >
                <span
                  class="carousel-control-next-icon"
                  aria-hidden="true"
                ></span>
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
          <a
            href="https://www.linkedin.com/in/paulo-henrique-almeida-silva-9234171b3/"
            title="Meu Linkedin"
          >
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
import ProjetosComponents from "@/components/ProjetosComponents.vue";

export default {
  name: "HomeView",
  components: { ProjetosComponents },
};
</script>