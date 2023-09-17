<template>
  <v-app>
    <default-bar />

    <default-view />
  </v-app>
</template>

<script lang="ts" setup>
  import DefaultBar from './AppBar.vue'
  import DefaultView from './View.vue'
</script>

<style lang="scss">
body{
  max-width: 640px;
  margin: auto;
}
.v-toolbar__content{
  max-width: 640px;
  margin: auto;
}
</style>
