<script setup>
import { withBase } from 'vitepress'

const props = defineProps({
  src: String,
  title: String
})

const videoUrl = withBase(props.src)

</script>
<template>
  <a :href="videoUrl" target="_blank" rel="noopener noreferrer">
    {{ title }}
  </a>
</template>