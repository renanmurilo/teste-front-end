<template>
    <section id="conteudo">
        <div class="container">
            <h2>Tinyone features</h2>
            <p class="sub-title">Lorem ipsum dolor sit amet, consectetur adipiscing elit. Praesent vitae eros eget tellus tristique bibendum. Donec rutrum sed sem quis venenatis.</p>
            <div class="session-conteudo">
                <div class="conteudo" v-for="(conteudo, index) in conteudos" :key="index">
                    <div class="image-icon">
                        <img :src="conteudo.image" alt="">
                    </div>
                    <div class="texto-conteudo">
                        <h3>{{ conteudo.title }}</h3>
                        <p>{{ conteudo.texto }}</p>
                    </div>
                </div>
                <div class="conteudo-2" v-for="(conteudo, index) in conteudo2" :key="index">
                    <div class="image-icon">
                        <img :src="conteudo.image" alt="">
                    </div>
                    <div class="texto-conteudo">
                        <h3>{{ conteudo.title }}</h3>
                        <p>{{ conteudo.texto }}</p>
                    </div>
                </div>
            </div>
        </div>
    </section>
</template>

<script>
export default {
    name: "Conteudo",

    data() {
    return {
      conteudos: [
        {
          id: 0,
          title: "Fully Responsive",
          texto: "Lorem ipsum dolor sit amet, consectetur adipiscing elit. Praesent vitae eros eget tellus tristique bibendum.",
          image: "./images/tablet.png"
        },
        {
          id: 1,
          title: "Fully Layered PSD",
          texto: "Lorem ipsum dolor sit amet, consectetur adipiscing elit. Praesent vitae eros eget tellus tristique bibendum.",
          image: "./images/lemon.png"
        },
        {
          id: 2,
          title: "Font Awesome Icons",
          texto: "Lorem ipsum dolor sit amet, consectetur adipiscing elit. Praesent vitae eros eget tellus tristique bibendum.",
          image: "./images/pasta.png"
        }
      ],
      conteudo2:[
        {
          id: 0,
          title: "HTML3 & CSS3 ",
          texto: "Lorem ipsum dolor sit amet, consectetur adipiscing elit. Praesent vitae eros eget tellus tristique bibendum.",
          image: "./images/html.png"
        },
        {
          id: 1,
          title: "Email Template",
          texto: "Lorem ipsum dolor sit amet, consectetur adipiscing elit. Praesent vitae eros eget tellus tristique bibendum.",
          image: "./images/envelope.png"
        },
        {
          id: 2,
          title: "Free to download",
          texto: "Lorem ipsum dolor sit amet, consectetur adipiscing elit. Praesent vitae eros eget tellus tristique bibendum.",
          image: "./images/bookmarks.png"
        }
      ]
    };
  },
}
</script>

<style scoped>
#conteudo{
    width: 100%;
    margin-top: 7rem;
    margin-bottom: 8rem;
}

#conteudo .container{
    max-width: 933px;
}

#conteudo h2{
    font-size: 32px;
    font-weight: bold;
    text-align: center
}

#conteudo .sub-title{
    max-width: 735px;
    text-align: center;
    font-size: 20px;
    margin: 1rem auto;
    font-weight: 300;
}

#conteudo .session-conteudo{
    margin-top: 76px;
    display: flex;
    justify-content: space-between;
    flex-wrap: wrap;
    align-items: center;
}

#conteudo .session-conteudo .conteudo{
    display: flex;
    align-items: space-betweem;
    margin-bottom: 5rem;
    margin-left: 1rem;
}

#conteudo .session-conteudo .conteudo-2{
    display: flex;
    align-items: space-betweem;
    margin-bottom: 1rem;
}

#conteudo .session-conteudo .conteudo .texto-conteudo,
.conteudo-2 .texto-conteudo{
    margin-left: 1rem;
}


#conteudo .session-conteudo .conteudo .texto-conteudo h3,
.conteudo-2 .texto-conteudo h3{
    font-size: 22px;
    counter-reset: #000;
    margin-bottom: 1rem;
}

#conteudo .session-conteudo .conteudo .texto-conteudo p,
.conteudo-2 .texto-conteudo p{
    font-size: 16px;
    color: #898989;
    max-width: 211px;
    line-height: 120%
}

@media screen and (max-width: 768px){

    #conteudo{
        margin-top: 3rem;
        margin-bottom: 3rem;
    }
    
    #conteudo .session-conteudo .conteudo, .conteudo-2{
        margin-left: auto;
        margin-right: auto;
        margin-bottom: 1rem;
    }
}
</style>