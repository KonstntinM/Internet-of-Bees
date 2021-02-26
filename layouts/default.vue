<template>
  <div>
    <NavigationBar />
    <SideBar />
    <Nuxt />
  </div>
</template>

<script>
import NavigationBar from '@/components/navigation/NavigationBar'
import SideBar from '@/components/navigation/SideBar'

export default {
  components: {
    NavigationBar,
    SideBar
  }
}
</script>

<style>

</style>
