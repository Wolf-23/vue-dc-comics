<template>
  <header class="container">
    <img src="../assets/images/dc-logo.png" alt="DC Logo">
    <ul>
        <li v-for="(link, index) in links" :key="index">
            <a :href="link.url" :class="link.active?'active':''">{{link.text}}</a>
        </li>
    </ul>
  </header>
</template>

<script>
export default {
    name: 'MyHeader',
    data() {
        return {
             links: [
                {
                    text: 'CHARACTERS',
                    url: '#',
                    active: false
                },
                {
                    text: 'COMICS',
                    url: '#',
                    active: true
                },
                {
                    text: 'MOVIES',
                    url: '#',
                    active: false
                },
                {
                    text: 'TV',
                    url: '#',
                    active: false
                },
                {
                    text: 'GAMES',
                    url: '#',
                    active: false
                }, 
                {
                    text: 'COLLECTIBLES',
                    url: '#',
                    active: false
                },
                {
                    text: 'VIDEOS',
                    url: '#',
                    active: false
                },
                {
                    text: 'FANS',
                    url: '#',
                    active: false
                },
                {
                    text: 'NEWS',
                    url: '#',
                    active: false
                },
                {
                    text: 'SHOP',
                    url: '#',
                    active: false
                }
            ]
        }
    }
}
</script>

<style scoped lang="scss">
    @import '../styles/general.scss';
    @import '../styles/vars.scss';
    header {
        display: flex;
        align-items: center;
        justify-content: space-between;
        height: 10vh;
        img {
            height: 70%;
        }
        li {
            list-style: none;
            display: inline-block;
            padding: 0 10px;
            a {
                text-decoration: none;
                color:black;
                font-weight: 600;
                font-size: 14px;
                &.active, &:hover {
                    color: $brand_color;
                }
            }    
        }
    }
</style>