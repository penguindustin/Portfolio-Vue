<template>
  <div>
    <p id="contact-header" class="light-green--text display-2">Hit me up :)</p>
    <div id="contact-links">
      <a
        href="https://github.com/penguindustin"
        target="_blank"
        class="badge badge-info"
        id="profile-link"
      >
        <i class="fab fa-github"></i> Github
      </a>
      <a href="https://twitter.com/Giant_Robato" target="_blank" class="badge badge-primary">
        <i class="fab fa-twitter"></i> Twitter
      </a>
      <a href="mailto:dustinmendoza64@gmail.com" class="badge badge-success">
        <i class="fas fa-envelope"></i> Email
      </a>
    </div>
    <div class="d-flex justify-center">
      <div
        class="light-green--text pa-5"
        v-for="contactData in contactInfo"
        :key="contactData.text"
      >
        <a :href="contactData.link">{{contactData.text}}</a>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data: () => ({
    contactInfo: [
      { link: "https://github.com/penguindustin", text: "Github" },
      { link: "https://twitter.com/Giant_Robato", text: "Twitter" },
      { link: "mailto:dustinmendoza64@gmail.com", text: "Email" }
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