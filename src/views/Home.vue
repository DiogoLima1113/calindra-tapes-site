<template>
  <div>
    <TopoHome/>
    <FimHome/>
  </div>
</template>

<script>
import TopoHome from '../components/TopoHome.vue';
import FimHome from '../components/FimHome.vue'

export default {
    name: 'Home',
    components: {
    TopoHome,
    FimHome,
  }
}
</script>

<style lang="scss" scoped>
</style>