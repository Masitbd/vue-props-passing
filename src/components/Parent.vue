<script setup>
import {reactive, provide} from 'vue'
import Child from './Child.vue'
const data = reactive({
message: 'Hello World'
})

provide('myData', data)

</script>

<template>
  <div>
    <h1>This is parent component</h1>
    <Child />
  </div>
</template>

<style lang="scss" scoped>


</style>