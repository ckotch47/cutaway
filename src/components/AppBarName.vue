<template>
  <span class="app-bar_name">{{nameTitle}}</span>
</template>

<script lang="ts">

export default {
  props: {
    nameTitle: String
  },
  name: "AppBarName"
}
</script>

<style scoped lang="scss">
.app-bar_name{
  margin-left: 5vw;
}
</style>
