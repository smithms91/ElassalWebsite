<template>
  <div id="app">
    <router-view />
    <footer-section />
  </div>
</template>

<script>
import FooterSection from './Footer'

export default {
  name: 'app',
  data () {
    return {

    }
  },
  components: {
    footerSection: FooterSection
  }
}
</script>

<style>
  *::before,
  *::after,
  * {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    outline: none;
  }
</style>
