<template>
<!--  :src =  v-bind:src -->
  <img :src="avatar" :alt="description">
</template>

<script>
export default {
  name: "Picture",
  data() {
    return {
      avatar: "/favicon.ico",
      description: "Vue do vitor"
    };
  },

}

</script>

<style scoped>

</style>