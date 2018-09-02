<template>
  <header class="mui-appbar mui--z1">
    <nav>
      <nuxt-link to="/">Home</nuxt-link>
      <nuxt-link to="/about">About</nuxt-link>
    </nav>
  </header>
</template>

<script>
  export default {
    name: 'appHeader'
  }
</script>

<style lang="css">
  header {
    box-sizing: border-box;
    background-color: #eee;
    border-top: 1px solid #e0e0e0;
    padding: .5em 0;
    display: flex;
    align-items: center;
  }

  .footer-flex-item {
    margin: .5em;
  }
</style>
