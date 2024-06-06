<script setup lang="ts">
const gitCommitSha = (import.meta.env.VITE_GIT_COMMIT_HASH || 'xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx').slice(0, 7)
const releaseVersion = import.meta.env.VITE_RELEASE_VERSION || 'v0.0.0'
</script>

<template>
  <div class="text-center text-xs">
    <span class="text-neutral-400">
      Powered by
    </span>
    <a href="https://github.com/zestaken" target="_blank">
      <span class="text-blue-500">
        泥电永远都队
      </span>
    </a>
    <!-- <span v-text="`${releaseVersion}-${gitCommitSha}`" /> -->
  </div>
</template>
