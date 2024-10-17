<template>
  <div>
    <div>
      <component-navbar></component-navbar>
      <div class="py-4">
        <router-view />
      </div>
      <component-footer></component-footer>
    </div>
  </div>
</template>

<script setup>
import ComponentNavbar from "./component-navbar.vue";
import ComponentFooter from "./component-footer.vue";
</script>

<style lang="scss" scoped></style>
