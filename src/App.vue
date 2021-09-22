<template>
  <!-- <v-app> -->
  <!-- <v-navigation-drawer class="green" app> -->
  <!-- <span class="white--text title">v-navigation-drawer</span> -->
  <!-- </v-navigation-drawer> -->
  <!-- <v-system-bar class="pink" app> -->
  <!-- <span class="white--text title">v-system-bar</span> -->
  <!-- </v-system-bar> -->
  <!-- <v-app-bar class="yellow" app> -->
  <!-- <span class="title">v-app-bar</span> -->
  <!-- </v-app-bar> -->
  <!-- <v-main class="blue"> -->
  <!-- <span class="white--text title">v-main</span> -->
  <!-- </v-main> -->
  <!-- <v-footer class="purple" app> -->
  <!-- <span class="white--text title mx-auto">v-footer</span> -->
  <!-- </v-footer> -->
  <!-- <v-bottom-navigation class="cyan" app> -->
  <!-- <span class="white--text title">v-bottom-navigation</span> -->
  <!-- </v-bottom-navigation> -->
  <!-- </v-app> -->

  <!-- <v-app>
    <v-app-bar class="blue" app>
      <v-app-bar-nav-icon class="white--text"></v-app-bar-nav-icon>
      <v-app-bar-title class="white--text">Layout Demo</v-app-bar-title>
    </v-app-bar>
    <v-main class="yellow lighten-4">
      <v-container class="mt-10" style="height: 300px">
        <v-toolbar dense>
          <v-btn icon>
            <v-icon>mdi-content-cut</v-icon>
          </v-btn>
          <v-btn icon>
            <v-icon>mdi-content-paste</v-icon>
          </v-btn>
          <v-btn icon>
            <v-icon>mdi-pencil-outline</v-icon>
          </v-btn>
          <v-btn icon>
            <v-icon>mdi-export-variant</v-icon>
          </v-btn>
          <v-spacer></v-spacer>
          <v-btn icon>
            <v-icon>mdi-dots-vertical</v-icon>
          </v-btn>
        </v-toolbar>
        <v-textarea
          outlined
          class="mt-10"
          label="My Statement"
          value="I wish I had learned Vuetify earlier!"
        ></v-textarea>
      </v-container>
    </v-main>
  </v-app> -->

  <v-app>
    <v-app-bar class="blue" app>
      <v-app-bar-nav-icon class="white--text"></v-app-bar-nav-icon>
      <v-app-bar-title class="white--text">Layout Demo</v-app-bar-title>
    </v-app-bar>
    <v-main class="yellow"> </v-main>
  </v-app>
</template>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Poppins:wght@500&display=swap');
a:not(active-class) {
  color: grey !important;
}
</style>

<script>
// import HelloWorld from './components/HelloWorld';

export default {
  name: 'App',
  data: () => ({}),
  components: {
    // HelloWorld,
  },
};
</script>
