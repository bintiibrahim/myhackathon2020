<template>
  <div
    class="min-h-screen flex items-center justify-center bg-gray-100 py-12 px-4 sm:px-6 lg:px-8"
  >
    <div class="max-w-md w-full">
      <div>
        <nuxt-link to="/">
          <img
            class="mx-auto h-12 w-auto"
            src="https://tailwindui.com/img/logos/workflow-mark-on-white.svg"
            alt="Workflow"
          />
        </nuxt-link>

        <h1
          class="mt-6 text-center text-5xl leading-9 font-extrabold text-gray-900"
        >
          Daftar akaun OKU
        </h1>
      </div>

      <div class="mt-20">
        <button
          @click="start()"
          class="group relative w-full flex justify-center py-8 px-4 border border-transparent text-2xl leading-5 font-medium rounded-md text-white bg-indigo-600 hover:bg-indigo-400 focus:outline-none focus:border-indigo-700 focus:shadow-outline-indigo active:bg-indigo-700 transition duration-150 ease-in-out"
        >
          Daftar
        </button>
        <p class="mt-8 text-center text-lg leading-5 text-gray-600">
          <nuxt-link
            to="/log-masuk"
            class="font-medium text-indigo-600 hover:text-indigo-500 focus:outline-none focus:underline transition ease-in-out duration-150"
          >
            Sudah ada akaun? Ketik sini.
          </nuxt-link>
        </p>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  methods: {
    start() {
      this.$router.push("/daftar/biodata");
    }
  }
};
</script>

<style scoped></style>
