<template>
  <div class="relative bg-white dark:bg-gray-800">
    <div class="flex flex-col sm:flex-row ml-12">
      <div class="min-w-full h-screen">
        <nav>
          <Element name="Dashboard" to="/" icon="home" />
          <Element name="Hives" to="/hives" icon="archive" />
          <Element name="Apiarys" to="/apiarys" icon="location-marker" />
          <Element name="Analytics" to="/analytics" icon="chart-pie" />
          <Element name="Settings" to="/settings" icon="cog" />
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
