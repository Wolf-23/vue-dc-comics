<template>
  <section>
    <div class="container">
        <h1>Content Goes Here</h1>
    </div>
  </section>
</template>

<script>
export default {
    name: 'MyContent'
}
</script>

<style scoped lang="scss">
  @import '../styles/mixins.scss';  

    section {
        background-color: #1C1C1C;
        height: 15vh;
        @include centering();
        h1 {
            color: #fff;
        }
    }
</style>