<template>
    <span>Brownie - 4 reais</span>
    <div>
        <button @click="diminuiContador">-</button>
        <span>{{ contador }}</span>
        <button @click="aumentaContador">+</button>
    </div>
</template>
<script setup>
import { ref } from 'vue'

const contador = ref(0);
const props = defineProps(['productName', 'productPrice'])

const diminuiContador = {} => {
    if(contador.value > 0) contador.value--;
}
const aumentaConador = {} => contador.value++;
</script>