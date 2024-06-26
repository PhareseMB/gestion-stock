<script setup>
import HelloWorld from './components/HelloWorld.vue'
import RegisterForm from './components/RegisterForm.vue'
</script>

<!-- src/App.vue -->
<template>
  <div id="app">
    <nav class="bg-neutral-500 p-4">
      <ul class="flex">
        <li class="mr-6">
          <router-link to="/register" class="text-white">Enregistrement</router-link>
        </li>
        <li>
          <router-link to="/login" class="text-white">Connexion</router-link>
        </li>
      </ul>
    </nav>
    <router-view></router-view>
  </div>
</template>

<script>
export default {
  name: 'App'
};
</script>

<style>
/*  */
</style>
