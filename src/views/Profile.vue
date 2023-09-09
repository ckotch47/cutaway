<template>

  <v-window
    v-model="window"

    flat
    rounded="0"
  >
    <v-window-item>
      <v-card class="mx-auto" >
        <v-img src="https://www.kare-design.com/wp-content/uploads/2015/08/2.jpg" cover max-height="60%"></v-img>
        <v-card-title>
          Top western road trips
        </v-card-title>

        <v-card-subtitle>
          1,000 miles of wonder
        </v-card-subtitle>
      </v-card>
      <v-card class="mx-auto" >
        <v-img src="https://www.kare-design.com/wp-content/uploads/2015/08/2.jpg" cover max-height="60%"></v-img>
        <v-card-title>
          Top western road trips
        </v-card-title>

        <v-card-subtitle>
          1,000 miles of wonder
        </v-card-subtitle>
      </v-card>
      <v-card class="mx-auto" >
        <v-img src="https://www.kare-design.com/wp-content/uploads/2015/08/2.jpg" cover max-height="60%"></v-img>
        <v-card-title>
          Top western road trips
        </v-card-title>

        <v-card-subtitle>
          1,000 miles of wonder
        </v-card-subtitle>
      </v-card>
    </v-window-item>

    <v-window-item>
     <link-list />
    </v-window-item>
  </v-window>

</template>

<script>
import LinkList from "../components/LinkList";
export default {
  name: "Profile",
  components: {LinkList},
  data: () => ({
    length: 3,
    window: 0,
  }),
}
</script>

<style scoped lang="scss">
.v-window{
  height: 100%;
}
.v-card{

  margin: 5vw;
}
</style>
