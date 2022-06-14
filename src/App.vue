<template>
  <v-app :dark="goDark">
    <v-content>
      <v-container align-center>
        <TheHeader :goDark="goDark" @changeTheme="updateTheme($event)"/>

        <transition
          name="router-animation"
          mode="out-in"
          enter-active-class="animated fadeIn fast"
          leave-active-class="animated fadeOut faster"
        >
          <router-view></router-view>
        </transition>
      </v-container>
    </v-content>
    <TheFooter/>
  </v-app>
</template>

<script>
import TheHeader from "./components/TheHeader";
import TheFooter from "./components/TheFooter";

export default {
  name: "App",
  metaInfo: {
    title: "Home",
    titleTemplate: "%s ← Yaseen Rashid",
    meta: [
      { name: "viewport", content: "width=device-width, initial-scale=1" },
      { name: "description", content: "Yaseen Rashid's Portfolio" },
      { charset: "utf-8" },
      { property: "og:title", content: "Yaseen' Rashid" },
      { property: "og:site_name", content: "Yaseen' Rashid" },
      { property: "og:type", content: "website" },
      { property: "og:url", content: "" },
      {
        property: "og:image",
        content: "https://lh3.googleusercontent.com/a-/AOh14Gi7bCiRRANzHRna_CiZLamWABhLpPlmVjC673Pk=s96-c-rg-br100"
      },
      { property: "og:description", content: "Yaseen Rashid's Portfolio" }
    ]
  },
  components: {
    TheHeader,
    TheFooter
  },
  data() {
    return { goDark: false };
  },
  methods: {
    updateTheme(updatedTheme) {
      this.goDark = !updatedTheme;
    }
  }
};
</script>
<style>
@import "https://cdnjs.cloudflare.com/ajax/libs/animate.css/3.7.0/animate.min.css";
</style>
