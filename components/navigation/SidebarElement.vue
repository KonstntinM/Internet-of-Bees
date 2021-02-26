<template>
  <a
    class="hover:text-gray-800 hover:bg-gray-100 flex items-center p-2 my-6 transition-colors dark:hover:text-white dark:hover:bg-gray-600 duration-200 rounded-lg"
    :class="{
      'text-gray-800 dark:text-gray-100 bg-gray-100 dark:bg-gray-600': isActive,
      'text-gray-600 dark:text-gray-400': '!isActive',
    }"
    :href="link"
  >
    <Icon :source="require(`~/assets/icons/heroicons/outline/${icon}.svg?raw`)" class="h-1/4 fill-current" />
    <span class="mx-4 text-lg font-normal"> {{ name }} </span>
    <span class="flex-grow text-right" />
  </a>
</template>

<script>
export default {
  props: {
    name: {
      type: String,
      required: true,
      default: 'Button'
    },
    link: {
      type: String,
      required: false,
      default: '#'
    },
    icon: {
      type: String,
      required: false,
      default: ''
    },
    notifications: {
      type: Number,
      required: false,
      default: 0
    },
    isActive: {
      type: Boolean,
      required: false,
      default: false
    }
  }
}
</script>

<style>
</style>
