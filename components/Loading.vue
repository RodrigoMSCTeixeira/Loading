<template>
  <div v-if="loading" class="loading-page">
    <div class="loading"></div>
  </div>
</template>

<script>
export default {
  data: () => ({
    loading: false
  }),

  methods: {
    start() {
      this.loading = true
    },
    finish() {
      this.loading = false
    }
  }
}
</script>

<style>
@import '~/static/css/loading.css';
</style>
