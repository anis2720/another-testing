<template>
  <div style="margin-bottom: 80px;" >
    <h1>Greetings!</h1>

    <div class="paragraph">
      <div>
        I'm <strong>Nurul Anis</strong>, a fresh graduate in Game Technology from Universiti Teknikal Malaysia Melaka (UTeM) with a strong passion for programming and game development. I have hands-on experience in developing interactive digital projects, including custom tools for environmental data monitoring and visualization, which reflect my ability to blend creativity with technical skill.
        </div>

        <div style="margin-top: 20px;">I've worked on  <router-link to="/game-projects">game projects</router-link>, on <router-link to="/other-projects">other projects</router-link>, and took part in <router-link to="/resume">a few things</router-link> as well.
        </div>

      <div style="margin-top: 40px;">I am eager to apply my knowledge and enthusiasm to real-world projects, particularly in game design, software development, and emerging technologies. Dedicated to continuous learning and professional growth, I am excited to contribute to the tech and digital innovation industry through meaningful, impactful work.
      </div>
    </div>

    <div class="photo">
      <img src="img/main-photo-bubble.png" alt="Avatar me" /> 
    </div>

    <div style="clear:both"></div>

  </div>
</template>

<style scoped>

a {
  color:#228B22;
  text-decoration: none;
  opacity: 1;
}
a:hover, .router-link-exact-active {
  color: #006400;
  text-decoration: underline;
  opacity: 1;
}

.paragraph {
  max-width: 700px;
  margin-bottom: 20px;
  backdrop-filter: blur(10px);
}

.photo {
  margin-top: 50px;
  text-align: center;
  image-rendering: auto;
}

@media only screen and (min-width: 620px){
  .paragraph {
    float: left;
  }

  .photo {
    float: left;
    padding: 10px;
    padding-left: 80px;
  }
}

</style>