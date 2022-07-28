<template>
  <div id="app">
    <Header />
    <Main />
  </div>
</template>

<script>

import BaseHeader from './components/BaseHeader.vue'
import TheMain from './components/TheMain.vue'

export default {
  name: 'Dc-Comics',
  components: {
    Header: BaseHeader,
    Main: TheMain,
  }
}
</script>

<style lang="scss">
@import './assets/scss/style.scss';

#app {
  height: 100vh;
}
</style>

