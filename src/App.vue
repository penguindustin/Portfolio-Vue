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

    <v-content>
      <Welcome />
      <HelloWorld />
    </v-content>
  </v-app>
</template>

<script>
import HelloWorld from "./components/HelloWorld";
import Welcome from "./components/Welcome";

export default {
  name: "App",

  components: {
    HelloWorld, Welcome
  },

  data: () => ({
    //
  })
};
</script>