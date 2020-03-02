<template>
  <v-card width="300" height="100%" class="mx-auto">
    <a :href="project.link">
      <v-img class="align-end" :src="project.imgSrc" max-height="200px"></v-img>
    </a>

    <v-card-title>
      <a :href="project.link">{{project.title}}</a>
    </v-card-title>

    <v-card-text class="text--primary">
      <div>{{project.blurb}}</div>
    </v-card-text>
  </v-card>
</template>

<script>
export default {
  props: ["project"],
  data: () => ({})
};
</script>

<style>
a {
  text-decoration: none;
}
</style>