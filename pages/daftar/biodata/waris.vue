<template>
  <div>
    <button
      class="mx-3 shadow bg-purple-500 hover:bg-purple-400 focus:shadow-outline focus:outline-none text-white font-bold py-2 px-4 rounded"
      @click="finish()"
    >
      Hantar permohonan
    </button>
  </div>
</template>

<script>
export default {
  layout: "biodata",
  data() {
    return {};
  },
  methods: {
    finish() {
      // TODO: Save to Vuex store

      this.$router.push("/daftar/tamat");
    }
  }
};
</script>

<style scoped></style>
