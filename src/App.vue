<template>
  <div id="app">
    <component :is="layout">
      <router-view/>  
    </component>
  </div>
</template>

<script>
import MainLayout from '@/layouts/MainLayout.vue'
export default {
  name: 'App',
  mounted() {
    console.log(this.$router)
  },
  computed: {
    layout () {
      return 'main-layout'
    }
  },
  components: {
    MainLayout
  }
}
</script>

<style lang="scss">
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
</style>
