<template>
  <section id="banner">
    <carousel 
        :perPage="1" 
        :loop="true" 
        :navigationEnabled="false" 
        :paginationEnabled="true" 
        :paginationSize="15" 
        :paginationPadding="5"
        :paginationActiveColor="[ffffff]"
    >
        <slide v-for="(slides, index) in slider" :key="index"> 
            <div class="image-banner">
                <img class="mobile" :src="slides.image" alt="">
                <h2>{{ slides.title }}</h2>
                <h3>{{ slides.subtitle }}</h3>
                <p>{{ slides.texto }}</p>
                <div class="icons">
                    <div>
                        <a href="#" to="/"><img src="../assets/apple.png" alt=""></a>
                    </div>
                    <div>
                        <a href="#" to="/"><img src="../assets/android.png" alt=""></a>
                    </div>
                    <div>
                        <a href="#" to="/"><img src="../assets/windows.png" alt=""></a>
                    </div>
                </div>
            </div>
        </slide>
    </carousel>
  </section>
</template>

<script>
import { Carousel, Slide } from "vue-carousel";

export default {
  name: "Banner",
 data() {
    return {
      slider: [
        {
          id: 0,
          title: "Inspire your inspiration",
          subtitle: "Simple to use for your app, products showcase and your inspiration",
          texto: "Lorem ipsum dolor sit amet, consectetur adipiscing elit. Praesent vitae eros eget tellus tristique bibendum. Donec rutrum sed sem quis venenatis. Proin viverra risus a eros volutpat tempor. In quis arcu et eros porta lobortis sit ",
          image: "./images/slide.png"
        },
        {
          id: 1,
          title: "Inspire your inspiration",
          subtitle: "Simple to use for your app, products showcase and your inspiration",
          texto: "Lorem ipsum dolor sit amet, consectetur adipiscing elit. Praesent vitae eros eget tellus tristique bibendum. Donec rutrum sed sem quis venenatis. Proin viverra risus a eros volutpat tempor. In quis arcu et eros porta lobortis sit ",
          image: "./images/slide.png"
        },
        {
          id: 2,
          title: "Inspire your inspiration",
          subtitle: "Simple to use for your app, products showcase and your inspiration",
          texto: "Lorem ipsum dolor sit amet, consectetur adipiscing elit. Praesent vitae eros eget tellus tristique bibendum. Donec rutrum sed sem quis venenatis. Proin viverra risus a eros volutpat tempor. In quis arcu et eros porta lobortis sit ",
          image: "./images/slide.png"
        }
      ]
    };
  },

  components: {
    Carousel,
    Slide
  }
};
</script>

<style scoped>
#banner{
  position: relative;
  width: 100%;
}

.image-banner{
    position: relative;
    background-size: cover;
    background-position: 100% 100%;
    background-repeat: no-repeat;
}

.image-banner h2{
    font-size: 32px;
    position: absolute;
    top: 13rem;
    font-weight: bold;
    left: 13rem;
    color: #000;
}

.image-banner h3{
    position: absolute;
    top: 16rem;
    left: 13rem;
    font-size: 20px;
    font-weight: 300;
    max-width: 380px;
    color: #313841;
}

.image-banner p{
    position: absolute;
    top: 20rem;
    left: 13rem;
    font-size: 16px;
    font-weight: 400;
    max-width: 398px;
    line-height: 120%;
    color: #555555;
}

.icons{
    position: absolute;
    display: flex;
    bottom: 13rem;
    left: 13rem;
}

.icons div{
    margin: 0 2rem 0 0;
}


@media screen and (min-width: 1441px) and (max-width: 1920px) {
  #banner .mobile{
    width: 1920px;
  }

  .image-banner h2{
    font-size: 48px;
    top: 18rem;
    left: 33rem;
  }

  .image-banner h3{
    top: 21rem;
    left: 33rem;
    font-size: 36px;
    max-width: 440px;
  }

  .image-banner p{
    top: 30rem;
    left: 33rem;
    font-size: 24px;
    max-width: 520px;
  }

  .icons{
    bottom: 19rem;
    left: 33rem;
  }
}

@media screen and (max-width: 1440px) {
  #banner .mobile{
    width: 1920px;
  }
}

@media screen and (max-width: 768px) {
  #banner{
    margin-top: 4.2rem
  }

  #banner .mobile{
    height: 350px;
    width: 100%;
  }

  .image-banner h2{
    font-size: 22px;
    top: 2rem;
    left: 1rem;
  }

  .image-banner h3{
    top: 4rem;
    left: 1rem;
    font-size: 16px;
    max-width: 188px;
  }

  .image-banner p{
    top: 8rem;
    left: 1rem;
    font-size: 12px;
    max-width: 188px;
  }

  .icons{
    bottom: 5rem;
    left: 1rem;
  }

  .icons div a img{
    width: 75%;
  }
}
</style>
