<template>
  <section>
    <div class="container">
      <ul>
        <li v-for="(bonus, index) in icons" :key="index">
          <img :src="bonus.icon" alt="Icona">
          <a :href="bonus.link">{{bonus.text}}</a>
        </li>
      </ul>
    </div>
  </section>
</template>

<script>
export default {
  name: 'MyBonus',
  data() {
    return {
      icons: [
        {
          icon: require('../assets/images/buy-comics-digital-comics.png'),
          text: 'DIGITAL COMICS',
          link: '#'
        },
        {
          icon: require('../assets/images/buy-comics-merchandise.png'),
          text: 'DC MERCHANDAISE',
          link: '#'
        },
        {
          icon: require('../assets/images/buy-comics-subscriptions.png'),
          text: 'SUBSCRIPTION',
          link: '#'
        },
        {
          icon: require('../assets/images/buy-comics-shop-locator.png'),
          text: 'COMIC SHOP LOCATOR',
          link: '#'
        },
        {
          icon: require('../assets/images/buy-comics-shop-locator.png'),
          text: 'DC POWER VISA',
          link: '#'
        }, 
      ]
    }
  }
}
</script>

<style scoped lang="scss">
  @import '../styles/vars.scss';
  @import '../styles/mixins.scss'; 
  section {
    background-color: $brand_color;
    height: 15vh;
    ul {
      display: flex;
      justify-content: space-around;
      li {
        list-style: none;
        @include centering();
        img {
          height: 30%;
        }
        a {
            text-decoration: none;
            color: #fff;
            font-size: 12px;
            padding-left: 10px;
        }    
      }
    }
  }
</style>