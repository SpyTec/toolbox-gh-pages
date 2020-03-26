<template>
  <div class="mx-6">
    <div class="flex p-10 items-start">
      <logo class="flex-initial w-6/12 mr-8" />
      <div class="flex-auto">
        <h1 class="font-display text-4xl leading-tight">
          Moderator Toolbox for Reddit
        </h1>
        <h2 class="font-display text-gray-700">
          Toolbox for Reddit is a Firefox and Chromium browser extension that provides a myriad of features and functionality to help Reddit moderators with their moderation work.
        </h2>
        <div class="font-body flex flex-row items-stretch m-4">
          <a
            href="https://addons.mozilla.org/en-US/firefox/addon/reddit-moderator-toolbox/"
            target="_blank"
            rel="noopener"
            class="browser-btn"
          >
            <img src="~/assets/firefox-logo.svg" class="w-16 mb-1">
            Mozilla Firefox
          </a>
          <a
            href="https://chrome.google.com/webstore/detail/moderator-toolbox-for-red/jhjpjhhkcbkmgdkahnckfboefnkgghpo"
            target="_blank"
            rel="noopener"
            class="browser-btn"
          >
            <img src="~/assets/chrome-logo.svg" class="w-16 mb-1">
            Google Chrome
          </a>
          <a
            href="https://microsoftedge.microsoft.com/addons/detail/nolhfmoadpbgfeonfnjlcfmhhkmdlfcl"
            target="_blank"
            rel="noopener"
            class="browser-btn"
          >
            <img src="~/assets/edge-logo.svg" class="w-16 mb-1">
            Microsoft Edge
          </a>
        </div>
      </div>
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
.browser-btn {
  @apply text-gray-900 flex flex-col items-center bg-white px-4 py-3 m-1 border-b-4 border-transparent
}
.browser-btn:hover {
  @apply border-blue-400
}
</style>
