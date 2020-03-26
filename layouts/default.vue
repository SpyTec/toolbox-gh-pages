<template>
  <div>
    <nav class="max-w-screen-xl mx-auto font-display flex pl-5 items-stretch justify-between">
      <nuxt-link to="/" class="flex-initial flex items-center mr-4 text-lg">
        <div class="flex-initial mr-2">
          <logo v-if="$route.name !== 'index'" class="w-8 mb-1" />
        </div>
        <a class="flex-initial">Toolbox</a>
      </nuxt-link>
      <div class="flex">
        <a
          href="https://github.com/toolbox-team/reddit-moderator-toolbox/releases"
          target="_blank"
          rel="noopener"
          class="flex-initial nav-link"
        >
          Releases
        </a>
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
    <div>
      <nuxt />
    </div>
    <div class="bg-gray-800 text-gray-300 text-sm">
      <tb-page class="grid sm:grid-cols-2 grid-cols-1 gap-2">
        <span class="align-center my-auto">
          Copyright 2020 - Toolbox team
        </span>
        <div class="flex flex-col">
          <h3 class="text-xl">Resources</h3>
          <ul>
            <li><a class="border-b-2 border-transparent hover:border-blue-400 hover:text-white" href="https://github.com/toolbox-team/reddit-moderator-toolbox" target="_blank" rel="noopener">GitHub</a></li>
            <li><a class="border-b-2 border-transparent hover:border-blue-400 hover:text-white" href="https://github.com/toolbox-team/reddit-moderator-toolbox/issues" target="_blank" rel="noopener">Issue Tracker</a></li>
          </ul>
        </div>
      </tb-page>
    </div>
  </div>
</template>

<script>
import Logo from '~/components/Logo.vue'
import TbPage from '~/components/TbPage.vue'

export default {
  components: {
    Logo,
    TbPage
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
.nav-link:active, .nav-link.nuxt-link-active {
  @apply border-blue-600
}
</style>
