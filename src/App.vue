<template>
  <div class="container">
    <header>
      <img alt="Vue logo" src="https://vuejs.org/images/logo.png" width="80" />
      <h1>Vue.js S3 Pipeline</h1>
      <p class="status">Status: <span class="badge">Online</span></p>
    </header>

    <main>
      <div class="card">
        <h2>🎉 Deploy Successful!</h2>
        <p>GitHub Actions + OIDC でデプロイされました。</p>
        
        <div class="counter-box">
          <p>Counter: {{ count }}</p>
          <button @click="count++">Click Me!</button>
        </div>
      </div>
    </main>
  </div>
</template>

<script setup>
import { ref } from 'vue'
const count = ref(0)
</script>

<style>
.container {
  font-family: 'Inter', system-ui, sans-serif;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
.card {
  background: white;
  border-radius: 12px;
  padding: 2rem;
  box-shadow: 0 4px 6px rgba(0,0,0,0.1);
  display: inline-block;
  margin-top: 2rem;
}
.badge {
  background: #42b883;
  color: white;
  padding: 4px 8px;
  border-radius: 4px;
  font-weight: bold;
}
button {
  background: #42b883;
  color: white;
  border: none;
  padding: 10px 20px;
  border-radius: 8px;
  cursor: pointer;
  font-size: 1rem;
}
button:hover { background: #33a06f; }
</style>