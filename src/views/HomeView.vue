<template>
  <div class="home">
    <img alt="Vue logo" src="../assets/logo.png">

    <div>
      <!-- <router-link :to="{ name: 'daybook' }" class="btn btn-primary">Daybook</router-link> -->
      <button @click="goToDaybook"  class="btn btn-primary">Primary</button>
      <button @click="goToDaybook" class="btn btn-secondary">Primary</button>
      <button @click="goToDaybook" class="btn btn-success">Primary</button>
    </div>
  </div>
</template>

<script>
export default {
  methods: {
    goToDaybook(){
      this.$router.push({ name: 'no-entry' })
    }
  }
}
</script>
