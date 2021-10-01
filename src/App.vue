<template>
  <div>
    <PrimeiroComponente />
    <LifeCycle />
    <Pessoa />
  </div>
</template>

<script>
import PrimeiroComponente from './components/PrimeiroComponente.vue'
import LifeCycle from './components/LifeCycle.vue'
import Pessoa from "@/components/Pessoa";

export default {
    name: 'App',
    components: { 
      PrimeiroComponente,
      LifeCycle,
      Pessoa,
    },
    data(){
      return{

      };
    },

}
</script>