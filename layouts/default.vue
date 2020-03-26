<template>
  <div>
    <nav class="max-w-screen-xl mx-auto font-display flex pl-5 items-stretch justify-between">
      <nuxt-link to="/" class="flex-initial flex items-center mr-4 text-lg">
        <div class="flex-initial mr-2">
          <logo v-if="$route.name !== 'index'" class="h-auto w-8 mb-1" />
        </div>
        <a class="flex-initial">Toolbox</a>
      </nuxt-link>
      <div class="flex">
        <nuxt-link to="/contribute" class="flex-initial nav-link">
          Contribute
        </nuxt-link>
        <a
          href="https://www.reddit.com/r/toolbox/wiki/index"
          target="_blank"
          rel="noopener"
          class="flex-initial nav-link"
        >
          Wiki
        </a>
        <nuxt-link to="/bar" class="flex-initial nav-link">
          Developers
        </nuxt-link>
      </div>
    </nav>
    <div class="max-w-screen-xl mx-auto">
      <nuxt />
    </div>
  </div>
</template>

<script>
import Logo from '~/components/Logo.vue'

export default {
  components: {
    Logo
  }
}
</script>

<style lang="postcss">
  .nav-link {
    @apply text-gray-700 text-center mx-2 px-2 pt-4 pb-2 border-b-4 border-transparent;
  }
  .nav-link:hover {
    @apply text-gray-900 border-blue-400;
  }
</style>
