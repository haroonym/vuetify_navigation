<template>
  <v-app>
    <v-app-bar class="blue" app>
      <v-app-bar-nav-icon @click.stop="drawer = !drawer" class="white--text"></v-app-bar-nav-icon>
      <span class="white--text title">Layout Demo</span>
    </v-app-bar>
    <v-navigation-drawer app hide-overlay disable-resize-watcher v-model="drawer">
      <v-btn text @click="drawer = false">Close</v-btn>

      <v-list-item-group>
        <v-list-item link v-for="(route, i) in routes" :key="i" :to="route.link" active-class="blue">
          {{ route.name }}
        </v-list-item>
      </v-list-item-group>
    </v-navigation-drawer>
    <v-main> <router-view></router-view></v-main>
  </v-app>
</template>

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
