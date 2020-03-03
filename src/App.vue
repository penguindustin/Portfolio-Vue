<template>
  <v-app>
    <v-app-bar app color="primary" dark absolute>
      <div class="d-flex align-center"></div>

      <v-spacer></v-spacer>

      <v-btn href="#welcome-section" target="_blank" text class="px-2">
        <span class="mr-2 headline">About</span>
      </v-btn>
      <v-btn href="#projects" target="_blank" text class="px-2">
        <span class="mr-2 headline">Work</span>
      </v-btn>
      <v-btn href="" target="_blank" text class="px-2">
        <span class="mr-2 headline">Contact</span>
      </v-btn>
    </v-app-bar>

    <v-content id="content">
      <Welcome />
      <Projects />
      <Contact />
    </v-content>
  </v-app>
</template>

<script>
import Welcome from "./components/Welcome";
import Projects from "./components/Projects";
import Contact from "./components/Contact";

export default {
  name: "App",

  components: {
    Welcome, Projects, Contact
  },

  data: () => ({
    //
  })
};
</script>

<style>
#content {
  background: #000;
}
</style>