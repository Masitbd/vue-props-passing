<script setup>
import {reactive, ref} from 'vue'
import ChildComponent from './ChildComponent.vue'
const data = reactive({
message: 'Hello World'
})

const getData = ref('')

const handleEvent = (message)=>{
  getData.value = message
}

</script>

<template>
  <div>
    <h1>This is parent component</h1>
    <ChildComponent :data="data" @myData = "handleEvent" />
    <p>Emitted message from ChildComponent: {{ getData }}</p>
    </div>
</template>

<style lang="scss" scoped>


</style>