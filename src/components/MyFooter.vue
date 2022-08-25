<template>
  <footer>
    <div class="footer-top">
      <div class="container">
        <div class="left">
          <div class="comics-shop">
            <h3>DC COMICS</h3>
            <ul>
              <li><a href="#">Characters</a></li>
              <li><a href="#">Comics</a></li>
              <li><a href="#">Movies</a></li>
              <li><a href="#">TV</a></li>
              <li><a href="#">Games</a></li>
              <li><a href="#">Videos</a></li>
              <li><a href="#">News</a></li>
            </ul>
            <h3>SHOP</h3>
            <ul>
              <li><a href="#">Shop DC</a></li>
              <li><a href="#">Shop DC Collectibles</a></li>
            </ul>
          </div>
          <div class="dc">
            <h3>DC</h3>
            <ul>
              <li><a href="#">Theme of Use</a></li>
              <li><a href="#">Privacy policy (new)</a></li>
              <li><a href="#">Ad Choises</a></li>
              <li><a href="#">Advertising</a></li>
              <li><a href="#">Jobs</a></li>
              <li><a href="#">Subscriptions</a></li>
              <li><a href="#">Talent Workshops</a></li>
              <li><a href="#">CPSC Certificates</a></li>
              <li><a href="#">Ratings</a></li>
              <li><a href="#">Shop Help</a></li>
              <li><a href="#">ContCT Us</a></li>
            </ul>
          </div>
          <div class="sites">
            <h3>SITES</h3>
            <ul>
              <li><a href="#">DC</a></li>
              <li><a href="#">MAD Magazine</a></li>
              <li><a href="#">DC Kids</a></li>
              <li><a href="#">DC Universe</a></li>
              <li><a href="#">DC Power Visa</a></li>
            </ul>
          </div>
        </div>
        <div class="right">
          <img src="../assets/images/dc-logo-bg.png" alt="Logo DC">
        </div>
      </div>
    </div>
    <div class="footer-bottom">
      <div class="container">
        <a href="#">SIGN-UP NOW!</a>
        <div class="follow">
          <h3>FOLLOW US</h3>
          <img src="../assets/images/footer-facebook.png" alt="Facebook">
          <img src="../assets/images/footer-twitter.png" alt="Twitter">
          <img src="../assets/images/footer-youtube.png" alt="Youtube">
          <img src="../assets/images/footer-pinterest.png" alt="Pinterest">
          <img src="../assets/images/footer-periscope.png" alt="Periscope">
        </div>
      </div>
    </div>
  </footer>
</template>

<script>
export default {
    name: 'MyFooter'
}
</script>

<style scoped lang="scss">
  @import '../styles/vars.scss';
  @import '../styles/mixins.scss';
  .footer-top {
    background-image: url(../assets/images/footer-bg.jpg);
    background-repeat: no-repeat;
    background-size: cover;
    height: 45vh;
    overflow: hidden;
    .container {
      display: flex;
      justify-content: space-between;
      align-items: center;
      height: 100%;
    }
    .left {
      display: flex;
      .comics-shop, .dc, .sites {
        padding: 0 20px;
      }
      h3 {
        color: white;
        padding: 7px 0;
      }
      ul {
        list-style: none;
        padding: 5px 0;
        li {
          padding: 2px 0;
          a{
            text-decoration: none;
            color: gray;
            &:hover {
            color: $brand_color;
          }
          }
        }
      }
    }
    }

  // ------------------
  .footer-bottom {
    background-color: #303030;
    height: 15vh;
    z-index: 555;
    .container {
      height: 100%;
      display: flex;
      justify-content: space-between;
      align-items: center;
      a {
        border: 2px solid $brand_color;
        padding: 10px;
        text-decoration: none;
        color: white;
        &:hover {
          border: 2px solid #fff;
          color: $brand_color;
        }
      }
      .follow {
        display: flex;
        align-items: center;
        h3 {
          padding: 0 15px;
          color:$brand_color;
        }
        img {
          padding: 0 10px;
        }
      }
    }
  }
</style>