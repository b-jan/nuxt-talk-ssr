<template>
  <footer>
    <div class="mui-container mui--text-center">
      <div class="footer-flex-item">
        Made by <a href="https://twitter.com/baptjan" target="_blank">Baptiste JAN</a>
      </div>
      <div class="footer-flex-item">
        Check the <a href="https://github.com/b-jan/nuxt-talk-ssr" target="_blank">Github Repo</a>
      </div>
    </div>
  </footer>
</template>

<script>
  export default {
    name: 'appFooter'
  }
</script>

<style lang="css">
  footer {
    box-sizing: border-box;
    background-color: #eee;
    border-top: 1px solid #e0e0e0;
    padding: .5em 0;
    display: flex;
    align-items: center;
    position: fixed;
    bottom: 0;
    left: 0;
    right: 0;
    height: 65px;
    z-index: 99;
  }

  .footer-flex-item {
    margin: .5em;
  }
</style>
