<template>
  <div class="container">
    <div>
      <Logo />
      <h1 class="title">nuxt-boilerplate</h1>
      <div class="links">
        <a
          href="https://nuxtjs.org/"
          target="_blank"
          rel="noopener noreferrer"
          class="drm-btn color-gray color-outlined size-lg"
        >
          Documentation
        </a>
        <a
          href="https://github.com/nuxt/nuxt.js"
          target="_blank"
          rel="noopener noreferrer"
          class="drm-btn color-green color-outlined size-lg"
        >
          GitHub
        </a>
        <NuxtLink
          to="/about"
          class="drm-btn color-green color-outlined size-lg"
        >
          About
        </NuxtLink>
      </div>
    </div>
  </div>
</template>

<script lang="ts">
import Vue from 'vue';
import Component from 'nuxt-class-component';

@Component
export default class IndexPage extends Vue {}
</script>

<style lang="scss">
.container {
  @apply mx-auto my-0 min-h-screen flex justify-center items-center text-center;
}

.links,
.title {
  @apply mt-5;
}

.links :not(:first-child) {
  @apply ml-5;
}
</style>
