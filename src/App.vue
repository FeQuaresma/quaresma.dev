<script setup lang="ts">
import githubIcon from "./assets/github-mark-white.svg";
import linkedinIcon from "./assets/linkedin-app-white-icon.webp";
import userIcon from "./assets/user.svg";
import projectsIcon from "./assets/rocket.svg";
import linkButton from "./components/link-button.vue";
</script>

<template>
  <div class="mainDiv">
    <img src="https://avatars.githubusercontent.com/u/96788382" class="photo" />

    <div class="textDiv">
      <h1>Felipe Quaresma</h1>
      <h2>Full-Stack Developer</h2>
    </div>

    <link-button
      :img-src="githubIcon"
      link="https://github.com/FeQuaresma"
      name="Github"
    />
    <link-button
      :img-src="linkedinIcon"
      link="https://www.linkedin.com/in/fequaresma/"
      name="Linkedin"
    />
    <link-button :img-src="userIcon" link="/about-me" name="About me" />
    <link-button :img-src="projectsIcon" link="/projects" name="Projects" />
  </div>
</template>

<style scoped>
.mainDiv {
  display: flex;
  flex-direction: column;
  gap: 1em;
  align-items: center;
}

.textDiv {
}

.photo {
  border-radius: 100%;
  height: 13em;
  width: 13em;
}
</style>
