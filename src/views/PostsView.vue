<template>
    <div class="posts">
      <img src="../assets/img/logo.svg" alt="antbook" class="logo">

      <CardComp class="mt-2 mx-auto single-post" parrafo="hello!!" picture="https://images.pexels.com/photos/206359/pexels-photo-206359.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=1" :header="{ name: 'Sebastian Maikol', picture: 'https://randomuser.me/api/portraits/men/81.jpg'}" :likes="true"/>

      <CardComp class="mt-2 mx-auto single-post" parrafo="HOLA!!" picture="https://images.pexels.com/photos/17568780/pexels-photo-17568780/free-photo-of-ciudad-punto-de-referencia-calle-edificios.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=1" :header="{ name: 'Susana Marea', picture: 'https://randomuser.me/api/portraits/women/81.jpg' }" :likes="true"/>
      
    </div>
</template>
<script>
  import CardComp from "../components/CardComp.vue"
  export default {
    name: "PostView",
    components: {
      CardComp
    }
  }
</script>

<style scoped>
  .posts{
    min-height: 60vh;
    max-width: 895px;
    margin: auto;
  }
  .logo{
    max-width: 115px;
    padding: 0.2rem;
  }
  .single-post{
    max-width: 550px;
  }
</style>