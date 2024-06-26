<script setup>
import HelloWorld from './components/HelloWorld.vue'
import RegisterForm from './components/RegisterForm.vue'
import Footer from './components/Footer.vue';
</script>

<!-- src/App.vue -->
<template>
  <div id="app">
    <nav class="bg-neutral-500 p-4">
      <ul class="flex">
        <li class="mr-6">
          <P class="rounded-md bg-gray-900 px-3 py-2 text-sm font-medium text-white font-bold">GESTION DE STOCK</p>
        </li>
        <li class="mr-6">
          <router-link to="/register" class="text-white">Enregistrement</router-link>
        </li>
        <li>
          <router-link to="/login" class="text-white">Connexion</router-link>
        </li>
      </ul>
    </nav>
    <router-view></router-view>
    <div>
      <Footer class="mt-40 ">
      <main class="flex-grow">
      <router-view></router-view>
    </main>
    </Footer>
    </div>
  </div>
  
</template>

<script>



export default {
  name: 'App',
  components: {
    Footer
  }
};
</script>

<style>
/*  */
</style>
