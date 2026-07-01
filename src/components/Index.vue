<template>
    <div>
        <button @click="isOpen = !isOpen">Toggle </button>
        <div v-show="isOpen">
            <h3>Premio</h3>
            <h3>Allion</h3>
            <h3>Corolla Fielder </h3>
            <h3>Axio</h3>
            <h3> Toyota Corolla </h3>
        </div>

    </div>
</template>

<script setup>

import { ref } from 'vue'

const isOpen = ref(false)
const toggle = ()=>{
    isOpen.value = !isOpen.value
}

</script>

<style lang="scss" scoped></style>