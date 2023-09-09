<template>
  <v-app-bar  :elevation="3" rounded>
    <v-app-bar-title>
      <v-avatar image="https://avatars.mds.yandex.net/get-kino-vod-films-gallery/28788/47e2fd514411e18b76af786d7417062d/380x240"></v-avatar>
      <app-bar-name :name-title="'someSome90'" />


    </v-app-bar-title>
    <v-btn icon="mdi-heart"></v-btn>

<!--    <v-btn icon="mdi-dots-vertical"></v-btn>-->
  </v-app-bar>
</template>

<script lang="ts">
import AppBarName from "@/components/AppBarName.vue";

export default {
  components: {AppBarName}
}
</script>
<style scoped lang="scss">
.v-app-bar.v-toolbar{
  box-shadow: none !important;
  background-color: #f7fcff;
}
</style>
