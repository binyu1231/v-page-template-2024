<script lang="ts" setup>

</script>

<template>
  <router-link
    v-bind="$attrs"
    class="cp-hyper-link"
  >
    <slot></slot>
  </router-link>
</template>

<style lang="postcss">
.cp-hyper-link {
  @apply text-sm font-medium text-purple-500 hover:text-purple-400 transition duration-150 ease-in-out ml-2;
}
</style>
