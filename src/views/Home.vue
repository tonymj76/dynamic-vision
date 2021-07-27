<template>
  <div>
    <div>
      <v-card width="100%" tile>
        <v-img
          src="@/assets/img/computer.jpg"
          height="500px"
          gradient="to top right, rgba(100,115,201,.33), rgba(25,32,72,.7)"
        >
          <v-row align="end" class="fill-height">
            <v-col align-self="center" class="px-12">
              <p class="text-h4 text-md-h3 text-lg-h2 white--text mt-12">
                WUYE Computer Literacy
              </p>
              <p class="text-h4 text-md-h3 text-lg-h2 white--text">
                Programme (WCLP 2021)
              </p>
              <p class="subtitle text-md-h5 mt-4">
                Become a computer literate today by enrolling in the “Computer
                Literacy for All Project 2030”
              </p>
              <v-card-actions class="pt-14">
                <v-btn
                  color="white lighten-2 pa-5 text-color"
                  x-large
                  @click="[]"
                >
                  Enroll Now
                </v-btn>
              </v-card-actions>
            </v-col>
          </v-row>
        </v-img>
      </v-card>
    </div>
    <div class="horro"></div>
  </div>
</template>

<script>
export default {
  name: "Home",
  components: {},
};
</script>

<style>
.subtitle {
  color: #f3f2f1;
}
.text-color {
  color: #456aa5 !important ;
  font-weight: bold;
}
</style>
