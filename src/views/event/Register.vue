<script setup>
import { useRouter } from 'vue-router'
const props = defineProps(['event'])
const router = useRouter()
const register = () => {
  // If registration successful
  router.push({
    name: 'EventDetails',
  })
}
</script>

<template>
  <p>Register event here</p>
  <button @click="register">Register Me!</button>
</template>
