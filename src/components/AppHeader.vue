<template>
  <b-navbar type="dark" variant="dark" class="d-flex flex-row">
    <b-navbar-nav class="flex-fill">
      <b-nav-item href="#"></b-nav-item>
    </b-navbar-nav>

    <b-navbar-nav class="ml-auto p-2">
      <router-link to="#section-team" v-slot="{navigate}">
        <b-button size="sm" variant="link" @click="navigate">Team</b-button>
      </router-link>
      <router-link to="#section-presentations-and-publications" v-slot="{navigate}">
        <b-button size="sm" variant="link" @click="navigate">Presentations and Publication</b-button>
      </router-link>
    </b-navbar-nav>
  </b-navbar>
</template>

<script>
export default {
  name: "AppHeader"
}
</script>

<style scoped>
button.btn {
  margin-left: 10px;
  margin-right: 10px;
}

button.btn-link {
  color: white;
  text-decoration: none;
}

button.btn-link:hover {
  text-decoration: underline;
}
</style>