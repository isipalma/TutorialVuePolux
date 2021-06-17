<template>
  <div>
    <input type="text" v-model="message">
    <p>{{ message }}</p>
  </div>
</template>

<script>
  export default {
    data() {
      return {
        message: ''
      }
    }
  }
</script>


<style scoped>
p {
  font-size: 2em;
  text-align: center;
}
</style>

