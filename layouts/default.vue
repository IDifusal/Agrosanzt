<template>
  <div class="app">
    <nav-bar />
    <Nuxt />
    <Bottom/>
  </div>
</template>
<script>
import NavBar from '~/components/NavBar.vue'
import Bottom from '~/components/Bottom.vue'
export default {
  components: { NavBar,Bottom },
  name: 'app',
}
</script>