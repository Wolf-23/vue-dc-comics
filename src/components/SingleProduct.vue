<template>
  <div class="single-product">
    <img :src="thumb" alt="Fumetto">
    <h5>{{name}}</h5>
  </div>
</template>

<script>
export default {
 name: "SingleProduct",
 props: {
    thumb: String,
    name: String
 }
}
</script>

<style scoped lang="scss">
    .single-product {
        img {
            width: 170px;
            height: 170px;
            object-fit: cover;
            object-position: top;
        }
        h5 {
            margin: 10px 0;
            color: #fff;
            text-transform: uppercase;
            font-weight: 100;
            font-size: 11px;
        }
    }
</style>