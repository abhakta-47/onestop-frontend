<template>
  <div class="container-fluid">
    <div class="row">
      <div class="col-2"></div>
      <div class="col-8">
        <div class="w-full max-w-xl">
          <form class="bg-black shadow-md rounded px-8 pt-6 pb-8 mb-4 mt-4">
            <div class="mb-4">
              <label
                class="block text-gray-700 text-sm font-bold mb-2"
                for="username"
              >
                Username
              </label>
              <input
                class="shadow appearance-none border rounded w-full py-2 px-3 text-gray-700 leading-tight focus:outline-none focus:shadow-outline"
                id="username"
                type="text"
                placeholder="Username"
                v-model="username"
              />
            </div>
            <div class="mb-6">
              <label
                class="block text-gray-700 text-sm font-bold mb-2"
                for="password"
              >
                Password
              </label>
              <input
                class="shadow appearance-none border border-red-500 rounded w-full py-2 px-3 text-gray-700 mb-3 leading-tight focus:outline-none focus:shadow-outline"
                id="password"
                type="password"
                v-model="password"
                placeholder="******************"
              />
              <p class="text-red-500 text-xs italic" v-if="password == ''">
                Please choose a password.
              </p>
            </div>
            <div class="flex items-center justify-between">
              <button
                class="bg-blue-500 hover:bg-blue-700 text-white font-bold py-2 px-4 rounded focus:outline-none focus:shadow-outline"
                type="button"
              >
                Sign In
              </button>
              <a
                class="inline-block align-baseline font-bold text-sm text-blue-500 hover:text-blue-800"
                href="#"
              >
                Forgot Password?
              </a>
            </div>
          </form>
          <p class="text-center text-gray-500 text-xs">
            &copy;2019 GNU/LINUX USER'S GROUP . All rights reserved.
          </p>
        </div>
      </div>
      <div class="col-2"></div>
    </div>
  </div>
</template>

<script>
import 'tailwindcss/dist/tailwind.min.css'

export default {
  data() {
    return {
      username: '',
      password: ''
    }
  }
}
</script>

<style scoped>
.container-fluid {
  width: 100vw!important;
  height: 100vh!important;
  background-color: black!important; 
}
.row {
  height: 100vh!important;
  background-color: rgb(27, 27, 27);
}
.col-8 {
  background: rgb(27, 27, 27);
}
form {
  word-break: break-all;
}
</style>