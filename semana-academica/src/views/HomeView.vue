<script setup>
import TheWelcome from '../components/TheWelcome.vue'
import ProductItem from '@/components/ProductItem.vue'

const nomeUsuario = ref('');
const nomeUsuario = ref('teste')

</script>

<template>
  <main>
    <div>
    <input type="text" v-model="nomeUsuario"/>
    <p>Olá, {{ nomeUsuario }}</p>
    </div>
    <ProductItem productName="Brownie" productPrice="4"/>
    <ProductItem productName="Guaravita" productPrice="2"/>
    <ProductItem productName="Água" productPrice="2"/>
  </main>
</template>
