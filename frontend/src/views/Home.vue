<template>
  <div class="home">
    <h2>登录功能可以写在这里</h2>
    <p>没有账号就注册一个</p>
  </div>
</template>

<script setup>
import { ref, onMounted } from 'vue'
import axios from 'axios'

const message = ref('')

onMounted(async () => {
  try {
    const response = await axios.get('/api/')
    message.value = response.data.message
  } catch (error) {
    console.error('Error fetching data:', error)
    message.value = 'Error connecting to backend'
  }
})
</script>

<style scoped>
.home {
  text-align: center;
  margin-top: 60px;
}

h2 {
  color: #2c3e50;
  margin-bottom: 20px;
}

p {
  color: #666;
  font-size: 16px;
}
</style> 