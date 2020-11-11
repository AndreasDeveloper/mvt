<template>
  <div id="app">
    <template v-if="!hasLayout">
       <Navbar />
    </template>
    <router-view/>
  </div>
</template>

<script>
import Navbar from '@/components/core/Navbar';

export default {
  components: {
    Navbar
  },
  computed: {
    hasLayout() {
      return this.$route.meta.hasLayout;
    },
  },
}
</script>

<style lang="scss">
@import './styles/main.scss';
</style>
