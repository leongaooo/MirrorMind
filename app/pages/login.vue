<template>
  <div class="login-page">
    <h1>登录</h1>
    <form @submit.prevent="handleLogin">
      <div class="form-group">
        <label for="username">用户名</label>
        <input id="username" v-model="username" type="text" required />
      </div>
      <div class="form-group">
        <label for="password">密码</label>
        <input id="password" v-model="password" type="password" required />
      </div>
      <button type="submit">登录</button>
    </form>
    <p @click="goToHome">返回首页</p>
  </div>
</template>

<script setup>
import { ref } from "vue";
import { navigateTo } from "nuxt/app";

const username = ref("");
const password = ref("");

const handleLogin = () => {
  // 这里添加登录逻辑
  console.log("登录信息:", {
    username: username.value,
    password: password.value,
  });
  // 登录成功后跳转到首页
  navigateTo("/");
};

const goToHome = () => {
  navigateTo("/");
};
</script>

<style scoped>
.login-page {
  max-width: 300px;
  margin: 50px auto;
  padding: 20px;
  border: 1px solid #ddd;
  border-radius: 8px;
}

.form-group {
  margin-bottom: 15px;
}

label {
  display: block;
  margin-bottom: 5px;
}

input {
  width: 100%;
  padding: 8px;
  border: 1px solid #ddd;
  border-radius: 4px;
}

button {
  width: 100%;
  padding: 10px;
  background-color: #007bff;
  color: white;
  border: none;
  border-radius: 4px;
  cursor: pointer;
}
</style>
