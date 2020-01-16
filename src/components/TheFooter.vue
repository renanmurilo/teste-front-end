<template>
  <footer>
    <div class="container">
      <h2>Keep in touch with us</h2>
      <p class="sub-title">Lorem ipsum dolor sit amet, consectetur adipiscing elit. Praesent vitae eros eget tellus tristique bibendum. Donec rutrum sed sem quis venenatis.</p>

      <div class="session-footer">
        <form action="">
          <input type="text" placeholder="Enter your email to update" required>
          <button type="button">Submit</button>
        </form>
      </div>

      <div class="icons-footer">
        <div>
          <a href="#"><img src="../assets/facebook.png" alt=""></a>
        </div>
        <div>
          <a href="#"><img src="../assets/twitter.png" alt=""></a>
        </div>
        <div>
          <a href="#"><img src="../assets/google.png" alt=""></a>
        </div>
        <div>
          <a href="#"><img src="../assets/pinterest.png" alt=""></a>
        </div>
      </div>

      <div class="contato">
        <div class="endereco">
          <p class="end">HALOVIETNAM LTD <br> 66, Dang Van ngu, Dong Da Hanoi, Vietnam</p>
          <p class="mail"><a href="mailto:contact@halovietnam.com">contact@halovietnam.com</a></p>
          <p class="tel"><a href="tel:+844 35149182">+844 35149182</a></p>
        </div>

        <div class="links_1">
          <div><a href="#" to="/">Examples</a></div>
          <div><a href="#" to="/">Shop</a></div>
          <div><a href="#" to="/">License</a></div>
        </div>

        <div class="links_2">
          <div><a href="#" to="/">Contact</a></div>
          <div><a href="#" to="/">About</a></div>
          <div><a href="#" to="/">Privacy</a></div>
          <div><a href="#" to="/">Terms</a></div>
        </div>

        <div class="links_3">
          <div><a href="#" to="/">Download</a></div>
          <div><a href="#" to="/">Support</a></div>
          <div><a href="#" to="/">Documents</a></div>
        </div>

        <div class="links_4">
          <div><a href="#" to="/">Media</a></div>
          <div><a href="#" to="/">Blog</a></div>
          <div><a href="#" to="/">Forums</a></div>
        </div>

      </div>
    </div>
  </footer>
</template>

<script>
export default {
  name: "TheFooter"
};
</script>

<style scoped>
footer {
  display: flex;
  background-color: #000; 
  text-align: center;
  justify-content: center;
}

footer .container{
  max-width: 933px;
}

footer h2{
  font-size: 32px;
  margin-top: 6rem;
  color: #fcdb00;
  font-weight: bold;

}

footer .sub-title{
  max-width: 760px;
  font-size: 20px;
  color: #898989;
  margin: 0 auto
}

footer form{
  display: flex;
  justify-content: center;
  margin-top: 2rem;
  margin-bottom: 5rem;
}

footer form input{
  width: 64%;
  height: 50px;
  border-radius: 5px;
  border: none;
  padding-left: 1.2rem;
}

footer form input::placeholder{
  font-size: 16px;
}

footer form button{
  width: 128px;
  height: 50px;
  background-color: #fcdb00;
  text-transform: uppercase;
  color: #010101;
  font-weight: bold;
  text-align: center;
  border: none;
  border-radius: 5px;
  margin-left: 1.5rem;
}

footer .icons-footer{
  display: flex;
  justify-content: center;
  margin-bottom: 8.375rem;
}

footer .icons-footer div{
  margin: 0 1rem;
}

footer .contato{
  display: flex;
  justify-content: flex-start;
  flex-wrap: wrap;
  margin-bottom: 8.6875rem;
}

footer .contato .endereco{
  display: flex;
  justify-content: flex-start;
  flex-wrap: wrap;
  max-width: 190px;
  margin-right: 9rem;
}

footer .contato .endereco .end{
  text-align: left;
  color: #fff;
  line-height: 120%;
  font-size: 16px;
  padding-left: .2rem;
}

footer .contato .endereco p{
  margin-bottom: 0px;
}

footer .contato .endereco .mail a, .tel a{
  color: #fff;
  font-size: 16px;
  text-align: left;
  text-decoration: none;
}

footer .contato .links_1 div,
.links_2 div,
.links_3 div{
  margin-right: 5.3rem;
}

footer .contato .links_1 div a,
.links_2 div a,
.links_3 div a,
.links_4 div a{
  text-decoration: none;
  color: #fff;
  font-size: 16px;
  display: flex;
  justify-content: flex-start;
  flex-wrap: wrap;
}

@media screen and (max-width: 678px) {

  footer .icons-footer{
    margin-bottom: 4rem;
  }

  footer .contato{
    margin-bottom: 2rem;
  }

  footer .contato .endereco{
    margin-right: 2rem;
    margin-bottom: 2rem;
  }
  
}
</style>
