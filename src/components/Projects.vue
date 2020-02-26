<template>
  <div>
    <v-container fluid>
      <v-row>
        <v-col v-for="project in projects" :key="project.title" :lg="3">
          <v-card max-width="300" class="mx-auto">
            <v-img
              class="white--text align-end"
              width="300px"
              src="@/assets/jwt-site.png"
            >
            <!-- TODO: make the above stinking dynamic -->
              <v-card-title>{{project.title}}</v-card-title>
            </v-img>
            <v-card-text class="text--primary">
              <div>{{project.blurb}}</div>
            </v-card-text>
          </v-card>
        </v-col>
      </v-row>
    </v-container>
  </div>
</template>

<script>
import projectData from "../static/projects.json";

export default {
  data: () => ({
    projects: projectData.projects
  }),
  methods: {
  },
  created: function() {
    console.log(this.projects);
  },
  computed: {
    Background () {
      //Load all pngs
      return require('../assets/' + this.id + '.png')
    },
    jpgBackground () {
      //Load all pngs
      return require('../assets/' + this.id + '.jpg')
    }
  }
};
</script>

<style>
</style>