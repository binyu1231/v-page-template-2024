<script lang="ts" setup>

</script>

<template>
  <Highlighter class="flex gap-4 px-4">
    <HighlighterItem class="flex-1" v-for="i in 4">
      <BrandCard :brand-index="i" title="月活用户数" en-title="Monthy User" count="123456" unit="n/m" />
    </HighlighterItem>
  </Highlighter>
</template>

<style lang="postcss">
.brand-list {
  @apply;
}
</style>
