<template>
  <div class="home-page">
    <h1>Welcome to MirrorMind</h1>
    <p>这是首页内容</p>
    <button @click="goToLogin">前往登录页</button>
  </div>
</template>

<script setup>
const goToLogin = () => {
  navigateTo('/login')
}
</script>

<style scoped>
.home-page {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  min-height: 100vh;
  gap: 20px;
}
</style>