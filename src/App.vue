<template>
  <section class="app">
    <runai-header>
      <nav>
        <img alt="run-todo logo" class="logo" src="@/assets/imgs/logo.png" width="60" height="60" />
        <router-link to="/">Home</router-link> |
        <router-link to="/about">About</router-link>
      </nav>
    </runai-header>
    <main class="main-content">
      <router-view />
    </main>
  </section>
</template>

<script lang="ts">
import { defineComponent } from 'vue'
import RunaiHeader from './shared/components/runai-header/runai-header.vue'

export default defineComponent({
  props: {},
  components: {
    RunaiHeader
  },
  data() {
    return {}
  }
})
</script>
<style lang="scss" scoped>
@import './shared/assets/scss/_variables.scss';
@import './shared/assets/scss/_colors.scss';
@import './assets/scss/_variables.scss';

nav {
  width: 100%;
  height: 100%;
  display: flex;
  align-items: center;
  padding: 0 20px;
  font-size: 16px;
  gap: 10px;
}

nav a {
  color: $white;
}

nav a.router-link-exact-active {
  color: $primary-color;
}

nav a.router-link-exact-active:hover {
  background-color: transparent;
}

.main-content {
  padding: calc($header-height + 5px) 20px 0 20px;
}
</style>
