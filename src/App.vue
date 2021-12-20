<template>
  <div id="app">
    <h1>Shop</h1>
    <div class="products-container">
      <Product v-for="product in products" :key="product" :name="product.name" :price="product.price" :description="product.description" :image="product.image"/>
    </div>
  </div>
</template>

<script>

import Product from './components/Product.vue'
import tempImage from './assets/logo.png'

export default {

  name: 'App',
  data:()=>{
    return{
      products: [
        {name: "Gems", price: 1000, description: "500 Clash royale gems", image: tempImage},
        {name: "Money", price: 1, description: "$1 for $1", image: tempImage},
        {name: "A+", price: 100000, description: "Free A+ in Comp sci", image: tempImage}
      ]
    }
  },
  components: {
    Product
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
.products-container{
  display: flex;
  justify-content: space-around;
  flex-wrap: wrap;
  align-content: center;
  flex-direction: row;
}
</style>
