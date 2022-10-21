<script>

import HomeView from "./views/HomeView.vue";

export default {
  components: {HomeView},
  mounted() {
    const paragraphs = this.$el.querySelectorAll('p');
    paragraphs.forEach(paragraph => {
      paragraph.innerHTML = paragraph.innerHTML
          .replaceAll(/DisasterAWARE/g, "<a href='https://www.pdc.org/disasteraware/'>DisasterAWARE</a>")
          .replaceAll(/PDC/g, "<a href='https://www.pdc.org/'>PDC</a>");
    });
  }
}
</script>

<template>
  <HomeView></HomeView>
</template>

<style scoped>

</style>
