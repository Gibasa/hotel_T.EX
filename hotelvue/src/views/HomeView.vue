<template>
  <!DOCTYPE html>
  <html lang="pt-br">
    <head>
      <meta charset="UTF-8" />
      <meta http-equiv="X-UA-Compatible" content="IE=edge" />
      <meta name="viewport" content="width=device-width, initial-scale=1.0" />

      <title>Hotel Recanto dos Códigos</title>
    </head>
    <body>
      <main>
        <section class="box-sobre pb5">
          <article class="container">
            <h2 class="titulo-h2 courier">
              <router-link class="link-border-bottom" :to="{ path: '/sobre' }"> SOBRE O NOSSO HOTEL</router-link>
            </h2>

            <div class="img-sobre display-f justify-c pt3">
              <img src="@/assets/images/hotel-sobre.png" alt="FOTO DO HOTEL" />
              <div class="noto-sans">
                <p class="paragrafo">
                  O Hotel Recanto dos Códigos é o lugar perfeito para aqueles
                  que buscam uma fuga da agitação da cidade e um mergulho na
                  natureza e na praia. Localizado em uma região remota e
                  selvagem, o hotel oferece quartos com vistas panorâmicas da
                  paisagem natural circundante e da praia.
                </p>

                <p class="paragrafo">
                  Os hóspedes podem desfrutar de atividades ao ar livre, como
                  caminhadas, observação de pássaros, piqueniques na natureza e
                  banhos de sol na praia. O hotel também oferece uma piscina ao
                  ar livre com vista para o mar e um spa com tratamentos de
                  bem-estar inspirados na natureza.
                </p>

                <p class="paragrafo">
                  Para aqueles que desejam relaxar em um ambiente tranquilo, o
                  hotel oferece uma biblioteca com uma seleção de livros, assim
                  como uma sala de jogos com jogos de mesa e cartas. Há também
                  uma sala de cinema para assistir a filmes. Para aqueles que
                  ainda assim precisem trabalhar, o hotel oferece um ambiente
                  com internet de qualidade para que os hóspedes possam utilizar
                  caso necessitem, sem perder a conexão com a natureza e a
                  praia.
                </p>

                <p class="paragrafo">
                  Em resumo, o Hotel Recanto dos Códigos é o lugar perfeito para
                  aqueles que desejam se desligar do mundo, se conectar com a
                  natureza e aproveitar o mar. Com atividades ao ar livre,
                  quartos confortáveis e refeições saudáveis, os hóspedes podem
                  desfrutar de uma estadia relaxante e rejuvenescedora neste
                  oásis de bem-estar natural e praiano.
                </p>
                <router-link class="saiba-mais" :to="{ path: '/sobre' }">Saiba mais</router-link>
              </div>
            </div>
          </article>
        </section>

        <section class="box-acomodacoes pb5">
          <article class="container">
            <div class="cards-quartos">
              <div class="courier">
                <h2 class="titulo-h2">
                  <router-link class="link-border-bottom" :to="{ path: '/acomodacoes' }">
                  CONFIRA NOSSAS ACOMODAÇÕES</router-link>
                </h2>
              </div>
              <div class="quartos display-f justify-csb align-c pt3">
                <div id="quarto1" class="quartos-home"></div>
                <div id="quarto2" class="quartos-home"></div>
                <div id="quarto3" class="quartos-home"></div>
              </div>
            </div>
          </article>
        </section>

        <section class="box-ilha">
          <article class="container">
            <div class="ilha display-f justify-c align-c">
              <h2 class="titulo-h2 courier">
                <a class="link-border-all" target="_blank" href="https://fundacaobaiaviva.org.br/baia-de-todos-os-santos/#principaisilhas">CONHEÇA A ILHA</a>
              </h2>
            </div>
          </article>
        </section>

        <section class="box-action">
          <article class="container">
            <div class="btn-conheca-mais noto-sans display-f justify-c">
              <router-link :to="{ path: '/acomodacoes' }">
                <button>Conheça mais sobre nossos serviços</button>
              </router-link>
            </div>
          </article>
        </section>

        <section class="box-gastronomia pb5">
          <article class="container">
            <div class="gastronomia">
              <h2 class="titulo-h2 courier">
                <a href="#" class="link-border-bottom">GASTRONOMIA</a>
              </h2>
              <div class="foto-texto-gastronomia display-f justify-c pt3">
                <img src="@/assets/images/gastronomia.jpg" alt="FOTO PRATO" />
                <div class="texto-gastronomia noto-sans">
                  <p class="paragrafo">
                    A gastronomia no Hotel Recanto dos Códigos é bastante
                    diversificada e de alta qualidade, oferecendo opções para
                    todos os gostos e paladares.
                  </p>
                  <p class="paragrafo">
                    O hotel possui um restaurante principal que oferece um café
                    da manhã com variedade de frutas frescas, pães, bolos,
                    iogurtes e outros itens. Almoço e jantar são servidos em um
                    buffet, com pratos quentes e frios, saladas, sopas e
                    sobremesas. Há também opções vegetarianas e veganas
                    disponíveis.
                  </p>
                  <p class="paragrafo">
                    Para os hóspedes que desejam algo mais íntimo, o hotel
                    oferece um serviço de quarto, com pratos preparados com
                    ingredientes frescos e locais. Os hóspedes também podem
                    desfrutar de drinks e coquetéis na piscina, no bar do hotel,
                    que possui uma vista panorâmica da praia e da natureza
                    circundante.
                  </p>
                  <p class="paragrafo">
                    O Recanto dos Códigos também oferece eventos especiais de
                    gastronomia, como jantares temáticos e degustações de vinhos
                    e queijos. Há também uma área de churrasco ao ar livre, onde
                    os hóspedes podem preparar suas próprias refeições.
                  </p>
                  <a class="saiba-mais" href="#">Saiba mais</a>
                </div>
              </div>
            </div>
          </article>
        </section>
      </main>
    </body>
  </html>
</template>

<script>
export default {
  name: "HomeView",
  components: {},
};
</script>
