<script setup lang="ts" generic="T extends any, O extends any">
defineOptions({
  name: 'Dashboard',
})

</script>

<template>
  <div class="flex gap-2">
    <RouterLink to="/access/signin">
      <div class="btn">登录</div>
    </RouterLink>
    <RouterLink to="/business/insight">
      <div class="btn">商业洞察</div>
    </RouterLink>
  </div>
</template>
