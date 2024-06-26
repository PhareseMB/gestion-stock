<template>
    <div class="max-w-md mx-auto mt-40 p-10 bg-white rounded-lg shadow-md">
      <div class="flex justify-center mb-6">
        <img src="../assets/nsia-logo.png" alt="Company Logo" class="h-16">
      </div>
      <h1 class="text-2xl font-bold mb-6 text-center">Formulaire d'enregistrement</h1>
      <form @submit.prevent="submitForm">
        <div class="mb-4">
          <label class="block text-gray-700 text-sm font-bold mb-2" for="nom">Nom</label>
          <input
            v-model="form.nom"
            type="text"
            id="nom"
            class="shadow appearance-none border rounded w-full py-2 px-3 text-gray-700 leading-tight focus:outline-none focus:shadow-outline"
            placeholder="Entrez votre nom"
          />
        </div>
        <div class="mb-4">
          <label class="block text-gray-700 text-sm font-bold mb-2" for="email">Email</label>
          <input
            v-model="form.email"
            type="email"
            id="email"
            class="shadow appearance-none border rounded w-full py-2 px-3 text-gray-700 leading-tight focus:outline-none focus:shadow-outline"
            placeholder="Entrez votre email"
          />
        </div>
        <div class="mb-4">
          <label class="block text-gray-700 text-sm font-bold mb-2" for="password">Password</label>
          <input
            v-model="form.password"
            type="password"
            id="password"
            class="shadow appearance-none border rounded w-full py-2 px-3 text-gray-700 leading-tight focus:outline-none focus:shadow-outline"
            placeholder="Entrez votre mot de passe"
          />
        </div>
        <div class="mb-4">
          <label class="block text-gray-700 text-sm font-bold mb-2" for="confirmPassword">Confirme Password</label>
          <input
            v-model="form.confirmPassword"
            type="password"
            id="confirmPassword"
            class="shadow appearance-none border rounded w-full py-2 px-3 text-gray-700 leading-tight focus:outline-none focus:shadow-outline"
            placeholder="Confirmez votre mot de passe"
          />
        </div>
        <div class="flex items-center justify-between">
          <button
            type="submit"
            class="bg-blue-950 hover:bg-amber-500 text-white font-bold py-2 px-4 rounded focus:outline-none focus:shadow-outline transition ease-in-out delay-150 hover:-translate-y-1 hover:scale-110  duration-300"
          >
            S'enregistrer
          </button>
        </div>
      </form>
    </div>
  </template>
  
  <script>
  export default {
    data() {
      return {
        form: {
          nom: '',
          email: '',
          password: '',
          confirmPassword: ''
        }
      };
    },
    methods: {
      submitForm() {
        // Logic for form submission
        console.log(this.form);
      }
    }
  };
  </script>
  
  <style scoped>
  /* Vous pouvez ajouter des styles supplémentaires ici */
  </style>


