<template>
  <main-layout-vue>
    <RouterView />
  </main-layout-vue>
</template>

<script>
import MainLayoutVue from './layout/MainLayout.vue'

export default {
  components: {
    MainLayoutVue,
  }
}
</script>