<template>
    <div class="max-w-md mx-auto mt-20 p-6 bg-white rounded-lg shadow-md">
      <div class="flex justify-center mb-6">
        <img src="../assets/nsia-logo.png" alt="Company Logo" class="h-16">
      </div>
      <h1 class="text-2xl font-bold mb-6 text-center">Formulaire de connexion</h1>
      <form @submit.prevent="submitLoginForm">
        <div class="mb-4">
          <label class="block text-gray-700 text-sm font-bold mb-2" for="email">Email</label>
          <input
            v-model="loginForm.email"
            type="email"
            id="email"
            class="shadow appearance-none border rounded w-full py-2 px-3 text-gray-700 leading-tight focus:outline-none focus:shadow-outline"
            placeholder="Entrez votre email"
          />
        </div>
        <div class="mb-6">
          <label class="block text-gray-700 text-sm font-bold mb-2" for="password">Mot de passe</label>
          <input
            v-model="loginForm.password"
            type="password"
            id="password"
            class="shadow appearance-none border rounded w-full py-2 px-3 text-gray-700 leading-tight focus:outline-none focus:shadow-outline"
            placeholder="Entrez votre mot de passe"
          />
        </div>
        <div class="flex items-center justify-between">
          <button
            type="submit"
            class="bg-blue-950 hover:bg-amber-500 text-white font-bold py-2 px-4 rounded focus:outline-none focus:shadow-outline transition ease-in-out delay-150 hover:-translate-y-1 hover:scale-110  duration-300"
          >
            Connexion
          </button>
        </div>
      </form>
    </div>
  </template>
  
  <script>
  export default {
    data() {
      return {
        loginForm: {
          email: '',
          password: ''
        }
      };
    },
    methods: {
      submitLoginForm() {
       //
        console.log(this.loginForm);
      }
    }
  };
  </script>
  
  <style scoped>
  /*.......................*/ 
  </style>
  