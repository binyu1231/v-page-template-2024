<script lang="ts" setup>
withDefaults(
  defineProps<{
    check?: boolean
  }>(),
  {
    check: false
  }
)
</script>

<template>
  <div class="cp-checkbox">
    <!-- -->
    <svg v-if="check" class="shrink-0" xmlns="http://www.w3.org/2000/svg" width="20" height="20">
      <path class="fill-purple-500" fill-opacity=".24" d="M10 0C4.5 0 0 4.5 0 10s4.5 10 10 10 10-4.5 10-10S15.5 0 10 0Z" />
      <path class="fill-purple-400" fill-rule="nonzero" d="M13 6.586 14.414 8l-5.747 5.748-3.081-3.081L7 9.252l1.667 1.667z" />
    </svg>
    <div v-else>

    </div>
  </div>
</template>

<style lang="postcss">
.cp-checkbox {
  @apply;
}
</style>
