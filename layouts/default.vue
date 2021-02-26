<template>
  <div>
    <NavigationBar />
    <div class="grid grid-flow-col grid-rows-1 grid-cols-5 gap-10 mt-10 px-6">
      <SideBar class="col-start-1" />
      <Nuxt class="col-start-2 col-end-6" />
    </div>
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
