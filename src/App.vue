<template>
  <main>
    <h1 class="contact-card">Mi Lista de Contactos</h1>
    <MiComponente 
      v-for="amigo in amigos" :key="amigo.id"
      :amigo="amigo" />
    
  </main>
</template>
  
<script>
import TarjetaContacto from '@/components/TarjetaContacto.vue';

export default {
  name: 'app',
  components: {
    MiComponente: TarjetaContacto
  },
  data(){
    return{
      amigos: [
        {
          id: 1,
          nombre: 'Rodrigo',
          descripcion: 'Desarrollador de software',
          imgSrc: 'https://cdn.pixabay.com/photo/2015/10/05/22/37/blank-profile-picture-973460_960_720.png',
        },
        {
          id: 2,
          nombre: 'Fernando',
          descripcion: 'Lider de Tomato',
          imgSrc: 'https://cdn.pixabay.com/photo/2015/10/05/22/37/blank-profile-picture-973460_960_720.png',
        },
        {
          id: 3,
          nombre: 'Alan',
          descripcion: 'Amigo de Fernando',
          imgSrc: 'https://cdn.pixabay.com/photo/2015/10/05/22/37/blank-profile-picture-973460_960_720.png',
        },
        {
          id: 4,
          nombre: 'Luis',
          descripcion: 'Mentor de Angular',
          imgSrc: 'https://cdn.pixabay.com/photo/2015/10/05/22/37/blank-profile-picture-973460_960_720.png',
        }
      ]
    }
  }
}
</script>

<style>
 
</style>
