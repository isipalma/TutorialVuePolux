<template>
  <div>
    <h1>Que buen mensaje</h1>
    <app-input></app-input>
  </div>
</template>

<script>
import Input from './Input.vue';
    export default {
        components: {
            'app-input': Input
        }
    }
</script>


<style scoped>
p {
  font-size: 2em;
  text-align: center;
}
</style>

