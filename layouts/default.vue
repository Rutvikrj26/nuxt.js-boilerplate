<template>
  <div
    :class="
      `site-layout-width-${$siteConfig.layout.width} posts-theme-${$siteConfig.posts.theme}`
    "
  >
    <site-nav />
    <nuxt />
  <div class="container">
    <Header />
    <ColorModePicker />
    <nuxt />
  </div>
    <site-footer></site-footer>
  </div>
</template>

<script>
import Header from '~/components/general/Header.vue'
import ColorModePicker from '~/components/general/ColorModePicker.vue'
import 'animate.css/animate.min.css'

export default {
  components: {
    Header,
    ColorModePicker
  }

}
</script>
