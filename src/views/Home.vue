<template>
  <div>
    <div>
      <v-card width="100%" tile>
        <v-img
          src="@/assets/img/computer.jpg"
          height="500px"
          gradient="to top right, rgba(100,115,201,.33), rgba(25,32,72,.7)"
        >
          <v-row align="end" class="fill-height ml-md-10">
            <v-col align-self="center" class="px-12 mt-16 pt-10">
              <p
                class="
                  text-h4 text-md-h3 text-lg-h2
                  white--text
                  font-weight-medium
                "
              >
                Dynamic Vision Computer
              </p>
              <p
                class="
                  text-h4 text-md-h3 text-lg-h2
                  white--text
                  font-weight-medium
                "
              >
                Project LTD (DVCP)
              </p>
              <p class="subtitle text-md-h5 mt-4 font-weight-medium">
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

    <section class="about--section">
      <v-container>
        <v-row justify="center">
          <v-col cols="12">
            <Header title="About Us" />
          </v-col>
          <v-col cols="12">
            <div>
              <p class="text-center body-1">
                Dynamic Vision Computer Project (DVCP) LTD is a global computer
                training/ICT firm with a powerful computer literacy and
                publication project. DVCP has a wide array of cooperate services
                that cuts across dynamic computer training, printing/
                publication, ICT corporation and computer maintenance services.
                DVCP is currently running a Computer Literacy for All Project
                2030 (CLAP 2030) in Nigeria with 70% hands-on practical
                sessions; with seasoned computer experts. In this global ICT age
                where computer literacy is a sin qua non, DVCP has a vision to
                increasing the computer literacy level with cutting age ICT
                knowledge in Nigeria by 60% in 2030.
              </p>
            </div>
          </v-col>
        </v-row>
      </v-container>
    </section>

    <section class="core--values">
      <v-container>
        <ServiceCard :core-value="coreData" />
      </v-container>
    </section>

    <section class="services">
      <v-container>
        <Header title="Our Services " />
        <div class="services-item">
          <div>
            <div>
              <img src="../assets/svg/publication.svg" alt="Publication" />
            </div>
            <div>
              <p class="text-center service-body font-weight-black">
                Publication
              </p>
            </div>
          </div>

          <div>
            <div>
              <img src="../assets/svg/consultancy.svg" alt="Training" />
            </div>
            <div>
              <p class="text-center service-body font-weight-black">Training</p>
            </div>
          </div>

          <div>
            <div>
              <img src="../assets/svg/publication.svg" alt="Partnership" />
            </div>
            <div>
              <p class="text-center service-body font-weight-black">
                Partnership
              </p>
            </div>
          </div>

          <div>
            <div>
              <img src="../assets/svg/consultancy.svg" alt="Consultancy" />
            </div>
            <div>
              <p class="text-center service-body font-weight-black">
                Consultancy
              </p>
            </div>
          </div>
        </div>
      </v-container>
    </section>

    <footer class="footer">
      <v-container>
        <v-row>
          <v-col>
            <h3 class="text-h4 footer--title">Location</h3>
            <p class="body-1 footer--body">
              Plot A287A Gbazango West Layout, <br />
              Annex II Kubuwa, Arab Road, Abuja
            </p>
          </v-col>
          <v-col>
            <h3 class="text-h4 footer--title">Contacts</h3>
            <p class="body-1 footer--body">
              +2348062430857
              <br />
              +2347031990128
            </p>
          </v-col>
        </v-row>
      </v-container>
    </footer>
  </div>
</template>

<script>
import ServiceCard from "@/components/ServiceCard";
import Header from "@/components/Header";
export default {
  name: "Home",
  components: {
    ServiceCard,
    Header,
  },
  computed: {
    coreData() {
      return [
        [
          "Our Vision",
          "Creating a world of  excellence with a strong computer literacy package; with a legacy to closing the computer knowledge gap in the 21st century.\n",
        ],
        [
          "Our Mission",
          "To increase the computer literacy level in Nigeria by 60% and exceptional computer services that meets global standard.",
        ],
        [
          "Our Core Values",
          "Vision Innovation Integrity Resilience Hard work Competence Excellence",
        ],
      ];
    },
  },
};
</script>

<style lang="scss">
.subtitle {
  color: #f3f2f1;
}
.footer {
  background: #456aa5;
  padding-top: 83px;
  padding-bottom: 83px;
  padding-left: 2rem;
  &--title {
    color: #f3f2f1 !important;
    padding-bottom: 2rem;
    font-style: normal;
    font-weight: 900;
    font-size: 40px !important;
    line-height: 47px;
  }
  &--body {
    color: #f3f2f1;
    font-style: normal;
    font-weight: 300;
    font-size: 28px;
    line-height: 35px;
  }
}
.about--section,
.services {
  padding-top: 7rem;
  padding-bottom: 3rem;
}

.services {
  height: 490px;
  background: #456aa50d;
  margin-top: 1rem;
  .service-body {
    font-size: 1.5rem !important;
  }
}
@media only screen and (min-width: 600px) {
  .services-item {
    display: flex;
    width: 50%;
    padding-top: 100px;
    margin: 0 auto;
    justify-content: space-between;
  }
}
.services-item {
  display: flex;
  width: 70%;
  padding-top: 60px;
  margin: 0 auto;
  justify-content: space-between;
}
.text-color {
  color: #456aa5 !important ;
  font-weight: bold;
}
</style>
