<template>
  <main>    
    <section class="contact-card">
      <img :src="amigo.imgSrc" alt="Imagen de perfil">
      <h2>{{ amigo.nombre }}</h2>
      <p>{{ amigo.descripcion }}</p>      
    </section>    
  </main>
</template>

<script>
export default {
  props: ['amigo']
}
</script>

<style scoped>
   .contact-card img{
    width: 100px;
    margin: 0 auto;
  }
  .contact-card {
    padding: 30px;
    margin: 30px;
    -webkit-box-shadow: -5px 10px 5px 0px rgba(0,0,0,0.118);
    -moz-box-shadow: -5px 10px 5px 0px rgba(0,0,0,0.118);
    box-shadow: -5px 10px 5px 0px rgba(0,0,0,0.118);
  }
</style>