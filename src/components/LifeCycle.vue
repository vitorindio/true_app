<template>
    <h1>meu nome é: {{nome}}</h1>
</template>

<script>

export default {
    name:'LifeCycle',
    data() {
        return{
            nome:'ainda não sei'
        }
        
    },
    created(){
        setTimeout(() =>{
            this.nome = 'Vitor'
        },  1000 );
    },

    mounted(){
      setTimeout(() =>{
            this.nome = 'joao'
      },    2000)
    },


}
</script>

<style scoped>

</style>