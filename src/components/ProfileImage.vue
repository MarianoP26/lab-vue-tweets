<script setup>

defineProps({
  image: {
    type: String,
    default: 'no img available',
  }
})

</script>

<template>
  <img :src="image" className="profile" alt="profile"/>
</template>

<style>

</style>