<template>
  <v-app>
    <v-toolbar
      app
      :clipped-left="clipped"
    >
      <v-toolbar-title v-text="title"></v-toolbar-title>
      <v-spacer></v-spacer>
      <v-avatar
          :tile="tile"
          :size="avatarSize"
          color="grey lighten-4"
        >
        <img src="/apple-touch-icon-180x180.png" alt="avatar">
      </v-avatar>
     
    </v-toolbar>
    <v-content>
      <router-view/>
    </v-content>
    <v-footer :fixed="fixed" app>
      <span>&copy; Pi 2018</span>
    </v-footer>
  </v-app>
</template>

<script>
export default {
  data() {
    return {
      title: "Game online"
    };
  },
  name: "App"
};
</script>
