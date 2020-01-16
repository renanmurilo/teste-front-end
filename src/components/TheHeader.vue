<template>
  <div class="container-fluid">
    <div class="row">
      <div class="col-12 p-0">
        <header>
          <div class="container">
              <b-navbar toggleable="lg">
                <b-navbar-brand>
                    <div><a href="#" to="/"><img src="../assets/logo-marca.png" alt=""></a></div>
                </b-navbar-brand>

                <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>

                <b-collapse id="nav-collapse" is-nav>
                    <b-navbar-nav>
                        <b-nav-item href="#" to="/">Features</b-nav-item>
                        <b-nav-item href="#" to="/">Support</b-nav-item>
                        <b-nav-item href="#" to="/">Blog</b-nav-item>
                    </b-navbar-nav>
                </b-collapse>
            </b-navbar>
          </div>
        </header>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "TheHeader"
};
</script>

<style scoped>

header {
  background-color: #fcdb00;
  padding-top: 60px;
  position: absolute;
  z-index: 1000;
  display: flex;
  justify-content: space-around;
  width: 100%;
}

header .container{
    max-width: 933px;
}

#nav-collapse {
  justify-content: flex-end;
}

li {
    padding-left: 39px;
}

.navbar-light .navbar-nav .nav-link {
  color: #000;
  font-weight: bold;
  letter-spacing: 1px;
  font-size: 22px;
}

li a {
  color: #000;
}

@media screen and (max-width: 768px) {
  header {
    padding-top: 10px;
  }
}
</style>
