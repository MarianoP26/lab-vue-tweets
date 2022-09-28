<script setup>

defineProps({
  message: {
    type: String,
    required: true,
  }
})
</script>

<template>
  <p className="message"> {{message}} </p>
</template>

<style>

</style>