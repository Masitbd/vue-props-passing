<script setup>

import {inject} from 'vue'

const data = inject('myData')

</script>

<template>
  <h1> {{ data.message }} comes from parent component</h1>
</template>



<style scoped>


</style>