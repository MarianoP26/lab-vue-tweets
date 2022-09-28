<script setup>

defineProps({
  name: {
    type: String,
    required: true,
  },
  handle: {
    type: String,
  }
})
</script>

<template>
  <span className="user">
    <span className="name"> {{name}} </span>
    <span className="handle">@ {{handle}}</span>
  </span>
</template>

<style>

</style>