<template>
  <div id="app">
    <the-header></the-header>
    <router-view></router-view>
    <the-footer></the-footer>
  </div>
</template>

<script>
  import TheHeader from './components/TheHeader.vue'
  import TheFooter from './components/TheFooter.vue'

  export default {
    name: 'App',
    components: {
      TheHeader: TheHeader,
      TheFooter: TheFooter
    }
  }
</script>
