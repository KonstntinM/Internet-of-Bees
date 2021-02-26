<template>
  <!-- eslint-disable-next-line vue/no-v-html -->
  <div v-html="source" />
</template>

<script>
/* eslint-disable */

export default {
  props: {
    source: {
      type: String,
      required: true,
      default: require('~/assets/icons/heroicons/outline/home.svg?raw')
    }
  }
}
</script>
