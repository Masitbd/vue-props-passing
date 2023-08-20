<script setup>
import {reactive, provide} from 'vue'
import ChildComponent from './ChildComponent.vue'
const data = reactive({
message: 'Hello World'
})

//provide('myData', data)

</script>

<template>
  <div>
    <h1>This is parent component</h1>
    <ChildComponent :data="data" />
  </div>
</template>

<style lang="scss" scoped>


</style>