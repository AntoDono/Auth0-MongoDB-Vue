<template>
  <div class="card">
    <div>
        <h1>{{ name }}</h1>
    </div>
    <div>
        <img :src="image"/>
    </div>
    <div>
        <p>
            {{ description }}
        </p>
    </div>
    <div>${{ price }}</div>
  </div>
</template>

<script>
export default {
  name: 'Products',
  
  props: {
    name: String,
    price: Number,
    description: String,
    image: Image
  },
  setup(props){
    console.log(props.name)
  },
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
    .card{
        border: 2px solid black;
        width: fit-content;
        padding: 2rem;
    }
</style>
