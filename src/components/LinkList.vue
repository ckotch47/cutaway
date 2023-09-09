<template>

  <v-list lines="three">
    <div
      v-for="folder in folders"
      :key="folder.title"
    >
    <v-list-item

      :title="folder.title"
      :subtitle="folder.subtitle"
    >

      <template v-slot:prepend>
        <v-avatar color="">

          <v-icon color="white" v-if="folder.icon.indexOf('mdi') !== -1" >{{folder.icon}}</v-icon>
          <v-img  height="64" :src="folder.icon"  v-else/>
        </v-avatar>
      </template>

    </v-list-item>
    <v-divider inset/>
    </div>
  </v-list>
</template>

<script>
export default {
  name: "LinkList",
  data: () => ({
    folders: [
      {
        subtitle: 'Номер телефона',
        title: '+7 (902) 751-93-60',
        icon: '/src/assets/icon/phone-call.svg'
      },
      {
        subtitle: 'Telegram',
        title: '@blant47',
        icon: '/src/assets/icon/telegram.svg'
      },
      {
        subtitle: 'О себе1',
        title: 'Some information about me',
        icon: 'mdi-information'
      },
    ],
  }),
}
</script>

<style scoped lang="scss">
i:before{
  color: black;
}
.v-list-item{
  padding: 3vw;
}
.v-img {
  .v-img__img {
    width: 32px;
    height: 32px;
    position: unset;
  }
}
</style>
