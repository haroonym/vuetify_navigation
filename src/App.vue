<template>
  <v-app>
    <v-app-bar class="grey lighten-5" height="74" app>
      <img class="mx-2" src="images/art.jpg" style="height:70px;" />
      <span class="text-truncate text-h4 blue-grey--text darken-1" style="font-family: Poppins"
        >Haroon Younas</span
      >
      <v-spacer></v-spacer>

      <v-btn
        class="grey accent-4 d-lg-block d-none"
        active-class="yellow accent-4"
        v-for="(route, i) in routes"
        :key="i"
        :to="route.link"
        exact
        elevation="2"
        large
        text
        style="margin-left: 15px;"
        >{{ route.name }}</v-btn
      >

      <v-app-bar-nav-icon class="black--text d-lg-none" @click="drawer = !drawer"></v-app-bar-nav-icon>
    </v-app-bar>

    <v-navigation-drawer app disable-resize-watcher right v-model="drawer">
      <v-btn text @click="drawer = false">Close</v-btn>
      <v-list-item-group class="d-lg-none">
        <v-list-item
          link
          v-for="(route, i) in routes"
          :key="i"
          :to="route.link"
          active-class="blue-grey lighten-4"
          >{{ route.name }}</v-list-item
        >
      </v-list-item-group>
    </v-navigation-drawer>
    <v-main>
      <div class="d-flex">
        <div style="width:250px"></div>
        <div class="mt-10" style="flex:1"><router-view></router-view></div>
      </div>
    </v-main>
  </v-app>
</template>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Poppins:wght@500&display=swap');
a:not(active-class) {
  color: green !important;
  padding-top: 15px !important;
}
</style>

<script>
export default {
  name: 'App',

  data: () => ({
    drawer: false,
    routes: [
      { name: 'Home', link: '/' },
      { name: 'About', link: '/about' },
      { name: 'Products', link: '/products' },
      { name: 'Team', link: '/team' },
    ],
  }),
};
</script>
