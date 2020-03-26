<template>
  <div>
    <div class="my-6">
      <tb-page>
        <logo class="flex-initial sm:w-64 w-16 mr-8" />
        <div class="flex-auto">
          <h1 class="font-display text-4xl leading-tight">
            Moderator Toolbox for Reddit
          </h1>
          <h2 class="font-display text-gray-700">
            Toolbox for Reddit is a Firefox and Chromium browser extension that provides a myriad of features and functionality to help Reddit moderators with their moderation work.
          </h2>
          <div class="font-body flex flex-row items-stretch m-4 whitespace-no-wrap">
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
      </tb-page>
    </div>
    <div class="bg-gray-200">
      <tb-page>
        <h2 class="text-3xl m-auto">Features</h2>
      </tb-page>
    </div>
    <div class="pb-2 bg-gray-200">
      <tb-page class="flex justify-between">
        <div class="flex-initial sm:mb-0 mb-5 sm:mr-12 mr-0 sm:w-auto w-full">
          <a
            href="https://www.reddit.com/r/toolbox/wiki/docs/removalreasons"
            target="_blank"
            rel="noopener"
          >
            <h2 class="text-2xl border-b-2 border-blue-400 hover:border-blue-600 mb-3">
              Removal reasons
            </h2>
          </a>
          <p>Gives you the ability to provide dynamic removals when removing items.</p>
          <ul class="list-disc list-outside ml-4 mt-2">
            <li>Subreddit specific removal reasons.</li>
            <li>Use dropdowns, checkboxes, and text inputs.</li>
            <li>Leave removal reasons as a comment, PM, or Modmail.</li>
          </ul>
        </div>
        <div class="flex-initial">
          <img src="~/assets/toolbox-features/removal-reasons.png" alt="Removal reasons" class="shadow-md">
        </div>
      </tb-page>
    </div>
    <div class="py-2">
      <tb-page class="flex flex-initial justify-between">
        <div class="flex-initial sm:mr-12 mr-0">
          <img src="~/assets/toolbox-features/mod-macro-add.png" alt="Mod macros" class="shadow-md">
        </div>
        <div class="flex-auto sm:mb-0 mb-5 sm:order-none order-first sm:w-auto w-full">
          <a
            href="https://www.reddit.com/r/toolbox/wiki/docs/removalreasons"
            target="_blank"
            rel="noopener"
          >
            <h2 class="text-2xl border-b-2 border-blue-400 hover:border-blue-600 mb-3">
              Mod macros
            </h2>
          </a>
          <p>Automation of actions through simple-to-use macros.</p>
          <ul class="list-disc list-outside ml-4 mt-2">
            <li>Usable for posts, comments, and new modmail.</li>
            <li>Executes all actions selected.</li>
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
.browser-btn {
  @apply text-gray-900 flex flex-col items-center bg-white px-4 py-3 m-1 border-b-4 border-transparent
}
.browser-btn:hover {
  @apply border-blue-400
}
.browser-btn:active {
  @apply border-blue-600
}
</style>
