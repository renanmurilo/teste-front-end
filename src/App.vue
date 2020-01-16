<template>
  <div id="app">
    <TheHeader />
      <transition mode="out-in">
        <router-view />
      </transition>
    <TheFooter />
  </div>
</template>

<script>
import TheHeader from "@/components/TheHeader.vue";
import TheFooter from "@/components/TheFooter.vue";

export default {
  components: {
    TheHeader,
    TheFooter
  }
};
</script>

<style>
@import url('https://fonts.googleapis.com/css?family=PT+Sans:400,700&display=swap');

* {
  box-sizing: border-box;
  font-family: 'PT Sans', sans-serif;
}

body,
ul,
li,
h1,
h2,
p {
  padding: 0px;
  margin: 0px;
}

a{
  text-decoration: none;
  color: #000000;
}

ul {
  list-style: none;
}

img {
  max-width: 100%;
  display: block;
}

.VueCarousel-pagination{
  position: absolute;
  bottom: 34px;
}

.VueCarousel-dot{
  opacity: .5;
}
.VueCarousel-dot--active{
  opacity: 1;
  background-color: #fff;
}

</style>
