<script lang="ts" setup>

</script>

<template>
  <button class="cp-button btn group" v-bind="$attrs">
    <slot></slot>
    <span class="cp-button-arrow group-hover:translate-x-0.5">-&gt;</span>
  </button>
</template>

<style lang="postcss">
.cp-button {
  @apply text-sm text-white bg-purple-500 hover:bg-purple-600 w-full shadow-sm ;
}

.cp-button-arrow {
  @apply tracking-normal text-purple-300 transition-transform duration-150 ease-in-out ml-1;
}
</style>
