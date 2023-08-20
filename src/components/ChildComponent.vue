<script setup>
import {ref} from 'vue'
defineProps(['data'])

const emit = defineEmits();


const messageEmitted = ()=>{

const eventData = 'pass data from chile to parent'  
emit('myData', eventData)

}

</script>

<template>
  <h1> {{ data.message }} comes from parent component</h1>
  <button @click="messageEmitted" class="bg-blue-500 hover:bg-blue-700 text-white font-bold py-2 px-4 rounded">
  Click me
</button>
</template>



<style scoped>


</style>