<script lang="ts" setup>
withDefaults(
  defineProps<{
    brandIndex?: number
    title: string
    enTitle: string
    count: number
    unit: string
  }>(),
  {
    brandIndex: 1
  }
)
</script>

<template>
  <div class="cp-brand-card">
    <!-- -->
    <div
      class="absolute bottom-0 translate-y-1/2 left-1/2 -translate-x-1/2 pointer-events-none -z-10 w-1/3 aspect-square"
      aria-hidden="true">
      <div
        class="absolute inset-0 translate-z-0 rounded-full bg-slate-800 group-[.swiper-slide-active]/slide:bg-purple-500 transition-colors duration-500 ease-in-out blur-[60px]">
      </div>
    </div>


    <div class="flex p-3 pr-6 h-full gap-2">
      <img :src="`/carousel-icon-0${brandIndex}.svg`" width="56" height="56" alt="Icon 01">
      <div class="grow">
        <div class="font-bold text-lg mb-1">{{ title }}</div>
        <GradientColorText class="font-700">{{ enTitle }}</GradientColorText>
      </div>
      <div class="flex items-end gap-1">
        <div class="text-4xl font-700">{{ count }}</div>
        <div class="mb-2 text-slate-4 font-700 text-lg">{{ unit }}</div>
      </div>
    </div>
  </div>
</template>

<style lang="postcss">
.cp-brand-card {
  @apply
  relative 
            h-full 
            border-1
            border-gray-700
      
            bg-slate-900 bg-opacity-60 rounded-[inherit] z-20 overflow-hidden;
}
</style>
