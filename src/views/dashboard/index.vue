<template>
  <div class="dashboard-container">
    <split></split>
  </div>
</template>

<script>
import { mapGetters } from 'vuex'
import split from './components/split.vue'

export default {
  components: { split },
  name: 'Dashboard',
  computed: {
    ...mapGetters([
      'name'
    ])
  }
}
</script>

<style lang="scss" scoped>
.dashboard-container {
  min-height: calc(100vh - 50px);
  margin: 50px 100px 50px 100px;
}
</style>
