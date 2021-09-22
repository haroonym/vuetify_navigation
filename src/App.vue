<template>
  <v-app>
    <v-app-bar class="grey lighten-5" height="74" app>
      <img class="mx-2" src="images/art.jpg" style="height:70px;" />
      <span class="text-truncate text-h4 blue-grey--text darken-1" style="font-family: Poppins"
        >Haroon Younas</span
      >
      <v-spacer></v-spacer>
      
      <v-btn class="grey accent-4" active-class="yellow accent-4" to="/" exact elevation="2" large text
        >Home</v-btn
      >
      <v-btn class="grey accent-4" active-class="yellow accent-4" to="/products" exact elevation="2" large text style="margin-left: 5px;"
        >Products</v-btn
      >
      <v-btn class="grey accent-4" active-class="yellow accent-4" to="/about" exact elevation="2" large text style="margin-left: 5px;"
        >About</v-btn
      >
    </v-app-bar>

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
  color: white !important;
}
</style>
