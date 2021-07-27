<template>
  <v-app>
    <v-app-bar app color="#F3F2F1" class="aligh-center justify-center">
      <div class="d-flex align-center">
        DVC
        <!-- <v-img
          alt="Vuetify Name"
          class="shrink mt-1 hidden-sm-and-down"
          contain
          min-width="100"
          src="https://cdn.vuetifyjs.com/images/logos/vuetify-name-dark.png"
          width="100"
        /> -->
      </div>

      <!-- <v-btn href="#" text>
        <span class="mr-2">Home</span>
      </v-btn> -->
    </v-app-bar>

    <v-main>
      <router-view />
    </v-main>
  </v-app>
</template>

<script>
export default {
  name: "App",

  data: () => ({
    //
  }),
};
</script>
