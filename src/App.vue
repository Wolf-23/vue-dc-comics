<template>
  <div id="app">
    <MyHeader/>
    <MyContent/>
    <MyBonus/>
    <MyFooter/>
  </div>
</template>

<script>
import MyHeader from './components/MyHeader.vue'
import MyContent from './components/MyContent.vue'
import MyFooter from './components/MyFooter.vue'
import MyBonus from './components/MyBonus.vue'

export default {
  name: 'App',
  components: {
    MyHeader,
    MyContent,
    MyFooter,
    MyBonus,
  }
}
</script>

<style lang="scss">
  @import './styles/general.scss';  
  @import './styles/vars.scss';  
  @import './styles/mixins.scss';  
</style>
