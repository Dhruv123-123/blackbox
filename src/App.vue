<template>
  <div class="bbp-page">
    <Blackbox :deep-links="true" source="https://github.com/Dhruv123-123/blackbox" />
  </div>
</template>

<script setup>
import Blackbox from '@/components/Blackbox/Blackbox.vue'
</script>

<style scoped>
.bbp-page { height: 100svh; width: 100vw; background: #0e1116; }
</style>
