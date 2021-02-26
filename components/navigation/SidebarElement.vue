<template>
  <NuxtLink
    :to="to"
    class="hover:text-gray-800 hover:bg-gray-100 flex items-center p-2 mb-5 transition-colors dark:hover:text-white dark:hover:bg-gray-600 duration-200 rounded-lg text-gray-600 dark:text-gray-400"
  >
    <Icon :source="require(`~/assets/icons/heroicons/outline/${icon}.svg?raw`)" class="h-1/4 fill-current" />
    <span class="mx-4 text-lg font-normal"> {{ name }} </span>
    <span class="flex-grow text-right" />
  </NuxtLink>
</template>

<script>
export default {
  props: {
    name: {
      type: String,
      required: true,
      default: 'Button'
    },
    to: {
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
    }
  }
}
</script>

<style scoped>
a.nuxt-link-exact-active {
  --tw-bg-opacity: 1;
  background-color: rgba(243, 244, 246, var(--tw-bg-opacity));
  --tw-text-opacity: 1;
  color: rgba(75, 85, 99, var(--tw-text-opacity));
}
</style>
