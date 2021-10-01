<template>
  <div>
    <p>opa novo componente com as info aqui!</p>
    <p v-if="esta_trabalhando" >to trabalhando com******* </p>
    <p v-else>Estou curtindo com*******</p>
    <ul>
     <li>vue/type</li>
     <li>java/groovy</li>
     <li>bootstrap/css</li>
    </ul>
    <div v-if="mostrar_email">
      <p>Mande uma mensagem para: {{email}} </p>
    </div>
    <div v-else>
      <p>perdeu!!</p>
    </div>
    <div>
      <p> para acessar a pag <a v-bind:href="meu_link" target="_blank">Clica ae!</a>
      </p>
      <Picture />
    </div>
  </div>
</template>

<script>
import Picture from "./Picture";

export default {
  name: "Info",
  components: {
      Picture,
  },
  data() {
    return{
      esta_trabalhando: null,
      mostrar_email: true,
      email: "vitor.indio@owse.com.br",
      meu_link:"https://google.com"
    };
  },
  /*init testes*/
  created(){
    setTimeout(() =>{
      this.esta_trabalhando = false
      this.mostrar_email= false
    },  4000 );
  },

  mounted(){
    setTimeout(() =>{
      this.esta_trabalhando = true
      this.mostrar_email = true
    },    8000)
  },
  /*end testes*/
}

</script>

<style scoped>

</style>