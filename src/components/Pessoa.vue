<template>
  <div>
    <p>____________________________</p>
    <h2>descriçao da pessoa : {{nome}} </h2>
    <p>esse componente acaba aqui!</p>
    <p>___________________________</p>

  <Info />
  <Form />

  </div>

</template>

<script>
import Info from "./Info";
import Form from "@/components/Form";

export default {
  name: 'Pessoa',
  components: {
    Info,
    Form,
  },
  data() {
    return{
      nome: 'Vitor'
    };
  },

}
</script>

<style scoped>

</style>