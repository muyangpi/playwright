<template>
  <div>
    <span data-testid="remount-count">{{ remountCount }}</span>
    <span data-testid="rerender-count">{{ count }}</span>
  </div>
</template>

<script lang="ts">
let remountCount = 0
</script>

<script lang="ts" setup>
defineProps({
  count: {
    type: Number,
    required: true
  }
})
remountCount++
</script>

