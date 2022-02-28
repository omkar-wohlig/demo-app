<template>
  <div class="center examplex">
    <vs-navbar center-collapsed v-model="active">
      <template #left>
        <img class="" src="../../public/store.svg" height="64" alt="" />
      </template>
      <vs-navbar-item :active="active == 'guide'" id="guide">
        Home
      </vs-navbar-item>
      <vs-navbar-item :active="active == 'docs'" id="docs">
        Order
      </vs-navbar-item>
      <vs-navbar-item :active="active == 'components'" id="components">
        Services
      </vs-navbar-item>
      <vs-navbar-item :active="active == 'license'" id="license">
        Contact
      </vs-navbar-item>
      <template #right>
        <vs-button flat>Login</vs-button>
        <vs-button>Get Started</vs-button>
      </template>
    </vs-navbar>
  </div>
</template>
  <script>
export default {
  data: () => ({
    active: "guide",
  }),
};
</script>