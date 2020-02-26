<template>
  <v-app>
    <v-app-bar app color="primary" dark>
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
      <HelloWorld />
    </v-content>
  </v-app>
</template>

<script>
import HelloWorld from "./components/HelloWorld";

export default {
  name: "App",

  components: {
    HelloWorld
  },

  data: () => ({
    //
  })
};
</script>