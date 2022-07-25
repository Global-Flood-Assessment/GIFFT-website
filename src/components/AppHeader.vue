<template>
  <b-navbar type="dark" variant="dark" class="d-flex flex-row">
    <b-navbar-nav class="flex-fill">
      <b-nav-item href="#"></b-nav-item>
    </b-navbar-nav>

    <b-navbar-nav class="ml-auto p-2">
      <b-button size="sm" variant="link">Menu 1</b-button>
      <b-button size="sm" variant="link">Menu 2</b-button>
      <b-button size="sm" variant="link">Menu 3</b-button>
      <b-button size="sm" variant="link">Menu 4</b-button>
      <b-button size="sm" variant="link">Menu 5</b-button>
      <b-button size="sm" variant="primary">Button</b-button>
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