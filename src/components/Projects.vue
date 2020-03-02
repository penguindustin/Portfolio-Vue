<template>
  <div>
    <v-container fluid>
      <v-row>
        <v-col v-for="project in projects" :key="project.title" :lg="3">
          <ProjectCard :project="project" />
        </v-col>
      </v-row>
    </v-container>
  </div>
</template>

<script>
import projectData from "../static/projects.json";
import ProjectCard from "../components/ProjectCard";

export default {
  components: {
    ProjectCard
  },
  data: () => ({
    projects: projectData.projects
  }),
  methods: {},
  computed: {}
};
</script>

<style>
a {
  text-decoration: none;
}
</style>