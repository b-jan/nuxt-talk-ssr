<template>
  <section class="container">
    <div>
      <AppLogo/>
      <h1 class="mui--text-display1">About Page</h1>
      <h1 class="mui--text-display1">(Nuxt SSR website)</h1>
      <h2 class="headline">Rendered From:<span class="render-result">{{renderSource}}</span></h2>
      <button
        id="reload-btn"
        class="mui-btn mui-btn--primary"
        @click="reloadPage">
        Reload Page
      </button>
    </div>
  </section>
</template>

<script>
  import AppLogo from '~/components/AppLogo.vue'

  export default {
    async asyncData () {
      return {
        renderSource: process.static ? 'static' : (process.server ? 'server' : 'client')
      }
    },
    components: {
      AppLogo
    },
    methods: {
      reloadPage () {
        window.location.reload()
      }
    }
  }
</script>
