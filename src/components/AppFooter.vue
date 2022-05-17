<template>
  <footer class="footer">
    <div class="footer__links">
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
    </div>
    <div class="footer__cta">
      <div class="container">
        <button>Sign-Up now !</button>
        <div class="social-links">
          <h2>Follow us</h2>
          <ul>
            <li>
              <a href="#"
                ><img src="../assets/img/footer-facebook.png" alt=""
              /></a>
            </li>
            <li>
              <a href="#"
                ><img src="../assets/img/footer-twitter.png" alt=""
              /></a>
            </li>
            <li>
              <a href="#"
                ><img src="../assets/img/footer-youtube.png" alt=""
              /></a>
            </li>
            <li>
              <a href="#"
                ><img src="../assets/img/footer-pinterest.png" alt=""
              /></a>
            </li>
            <li>
              <a href="#"
                ><img src="../assets/img//footer-periscope.png" alt=""
              /></a>
            </li>
          </ul>
        </div>
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
  &__links {
    background-image: url("../assets/img/footer-bg.jpg");
    background-size: cover;
    background-repeat: no-repeat;
  }
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
  &__cta {
    background-color: #303030;
    .container {
      height: $header-height;
      display: flex;
      justify-content: space-between;
      align-items: center;
      button {
        text-transform: uppercase;
        background-color: inherit;
        color: white;
        padding: 0.6rem;
        font-size: 1rem;
        border: 2px solid $brand-primary-color;
      }
      .social-links {
        display: flex;
        color: $brand-primary-color;
        ul {
          display: flex;
          margin-left: 0.5rem;
          li {
            margin: 0 0.5rem;
          }
        }
      }
    }
  }
}
</style>
