<script>

import HomeView from "./views/HomeView.vue";

export default {
  components: {HomeView},
  mounted() {
    this.$el.outerHTML = this.$el.outerHTML
        .replaceAll(/DisasterAWARE/g, "<a href='https://www.pdc.org/disasteraware/'>DisasterAWARE</a>")
        .replaceAll(/PDC/g, "<a href='https://www.pdc.org/'>PDC</a>");
  }
}
</script>

<template>
  <HomeView></HomeView>
</template>

<style scoped>

</style>
