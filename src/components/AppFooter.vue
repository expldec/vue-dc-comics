<template>
  <footer class="footer">
    <div class="container footer__container">
      <div class="footer__col">
        <h2>DC Comics</h2>
        <ul>
          <li><a href="#">Characters</a></li>
          <li><a href="#">Comics</a></li>
          <li><a href="#">Movies</a></li>
          <li><a href="#">TV</a></li>
          <li><a href="#">Games</a></li>
          <li><a href="#">Videos</a></li>
          <li><a href="#">News</a></li>
        </ul>
        <h2>DC Shop</h2>
        <ul>
          <li><a href="#">Shop DC</a></li>
          <li><a href="#">Shop DC Collectibles</a></li>
        </ul>
      </div>
      <div class="footer__col">
        <h2>DC</h2>
        <ul>
          <li><a href="#">Terms Of Use</a></li>
          <li><a href="#">Privacy Policy (New)</a></li>
          <li><a href="#">Advertising</a></li>
          <li><a href="#">Jobs</a></li>
          <li><a href="#">Subscriptions</a></li>
          <li><a href="#">CPSC Certificates</a></li>
          <li><a href="#">Ratings</a></li>
          <li><a href="#">Shop Help</a></li>
          <li><a href="#">Contact Us</a></li>
        </ul>
      </div>
      <div class="footer__col">
        <h2>Sites</h2>
        <ul>
          <li><a href="#">DC</a></li>
          <li><a href="#">DC UNIVERSE INFINITE</a></li>
          <li><a href="#">DC Kids</a></li>
          <li><a href="#">DC Shop</a></li>
          <li><a href="#">MAD Magazine</a></li>
        </ul>
      </div>
      <div class="footer__col-logo">
        <!-- <img src="../assets/img/dc-logo-bg.png" alt="" /> -->
      </div>
    </div>
  </footer>
</template>

<script>
export default {
  name: "AppFooter",
};
</script>

<style lang="scss" scoped>
@import "../style/variables.scss";
.footer {
  background-image: url("../assets/img/footer-bg.jpg");
  background-size: cover;
  background-repeat: no-repeat;
  &__container {
    display: flex;
  }
  &__col {
    padding: 3rem 1rem;
    h2 {
      font-size: 1.2rem;
      color: white;
      text-transform: uppercase;
      margin-bottom: 0.5rem;
    }
    ul {
      margin-bottom: 0.5rem;
    }
    a {
      color: $text-grey;
      font-size: 0.8rem;
    }
    &-logo {
      flex-grow: 1;
      background-image: url("../assets/img/dc-logo-bg.png");
      background-position: center;
      background-repeat: no-repeat;
    }
  }
  &__img {
    width: 70%;
  }
}
</style>
