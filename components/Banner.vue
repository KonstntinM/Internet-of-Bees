/* Based on https://tailwindui.com/preview */

<template>
  <div v-if="isVisible" class="bg-indigo-600">
    <div class="max-w-7xl mx-auto py-3 px-3 sm:px-6 lg:px-8">
      <div class="flex items-center justify-between flex-wrap">
        <div class="w-0 flex-1 flex items-center">
          <span class="flex p-2 rounded-lg bg-indigo-800">
            <Icon :source="require('~/assets/icons/heroicons/outline/speakerphone.svg?raw')" />
          </span>
          <p class="ml-3 font-medium text-white truncate">
            <span class="hidden md:inline">
              {{ message }}
            </span>
          </p>
        </div>
        <div
          class="order-3 mt-2 flex-shrink-0 w-full sm:order-2 sm:mt-0 sm:w-auto"
        >
          <a
            href="#"
            class="flex items-center justify-center px-4 py-2 border border-transparent rounded-md shadow-sm text-sm font-medium text-indigo-600 bg-white hover:bg-indigo-50"
          >
            {{ callToAction }}
          </a>
        </div>
        <div class="order-2 flex-shrink-0 sm:order-3 sm:ml-3">
          <button
            type="button"
            class="-mr-1 flex p-2 rounded-md hover:bg-indigo-500 focus:outline-none focus:ring-2 focus:ring-white sm:-mr-2"
            @click="isVisible = !isVisible"
          >
            <span class="sr-only">Dismiss</span>
            <Icon :source="require('~/assets/icons/heroicons/outline/x.svg?raw')" />
          </button>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  props: {
    message: {
      type: String,
      required: true,
      default: 'Oh, something went wrong here, unfortunately.'
    },
    callToAction: {
      type: String,
      required: false,
      default: 'Learn more'
    },
    href: {
      type: String,
      required: false,
      default: '/404'
    }
  },
  data: () => {
    return {
      isVisible: true
    }
  }
}
</script>
