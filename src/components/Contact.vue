<template>
  <div>
    <p id="contact-header" class="light-green--text display-2">Contact Me</p>
    <div class="d-flex justify-center">
      <div
        class="light-green--text pa-5 display-1"
        v-for="contactData in contactInfo"
        :key="contactData.text"
      >
        <a :href="contactData.link">
          <i :class="contactData.class"></i>
          {{contactData.text}}
        </a>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data: () => ({
    contactInfo: [
      {
        link: "https://github.com/penguindustin",
        text: "Github",
        class: "fab fa-github"
      },
      {
        link: "https://twitter.com/Giant_Robato",
        text: "Twitter",
        class: "fab fa-twitter"
      },
      {
        link: "mailto:dustinmendoza64@gmail.com",
        text: "Email",
        class: "fas fa-envelope"
      }
    ]
  })
};
</script>

<style>
#contact-header {
  text-align: center;
  display: block;
}
#contact-links {
  display: flex;
  justify-content: center;
  width: 100%;
  flex-wrap: wrap;
}
</style>