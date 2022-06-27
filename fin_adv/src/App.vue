<template>
<v-app>
  <v-navigation-drawer app color="red">
    <h1>Боковое меню</h1>
  </v-navigation-drawer>

  <v-app-bar app color="green">
    <v-col cols="4" class="ma-3">
      <v-autocomplete hide-details rounded solo dense>
      </v-autocomplete>
    </v-col>
    <v-spacer></v-spacer>
    <div class="d-flex justify-end">
      <div>
        <v-avatar color="red ma-3">
          <span class="white--text headline">AS</span>
        </v-avatar>
      </div>
      <div class="flex-column ma-3">
        <p class="ma-0 pa-0">Name Surname</p>
        <p class="ma-0 pa-0">Mail</p>
      </div>
    </div>
  </v-app-bar>

  <!-- Sizes your content based upon application components -->
  <v-main color="black">

    <!-- Provides the application the proper gutter -->
    <v-container fluid>
      <!-- If using vue-router -->
      <router-view></router-view>
    </v-container>
  </v-main>

  <v-footer app color="grey">
    <h1>Подвал</h1>
  </v-footer>
</v-app>
</template>
<script>

export default {
  name: 'App',
  components: {
  }
}
</script>