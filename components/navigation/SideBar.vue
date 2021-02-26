<template>
  <div class="relative bg-white dark:bg-gray-800">
    <div class="flex flex-col sm:flex-row ml-12">
      <div class="w-72 h-screen">
        <nav class="mt-10 px-6">
          <Element name="Dashboard" icon="home" :is-active="false" />
          <Element name="Hives" icon="archive" :is-active="false" />
          <Element name="Apiarys" icon="location-marker" :is-active="false" />
          <Element name="Analytics" icon="chart-pie" :is-active="false" />
          <Element name="Settings" icon="cog" :is-active="false" />
        </nav>
      </div>
    </div>
  </div>
</template>

<script>
import Element from '@/components/navigation/SidebarElement'

export default {
  components: {
    Element
  }
}
</script>

<style>
</style>
