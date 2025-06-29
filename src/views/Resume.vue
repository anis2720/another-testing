<template>
  <div>
    <h1>Resume</h1>

    <div class="paragraph">
      I'm <strong>Nurul Anis</strong>, a fresh graduate from Universiti Teknikal Malaysia Melaka (UTeM). From the very start of my studies in Game Technology, I was driven by a passion to blend programming skills with creative design. 
      Throughout my time at UTeM, I worked on various interactive digital projects, including developing custom tools for environmental data monitoring and visualization. 
      These experiences challenged me to think critically, explore innovative solutions, and strengthened my abilities in programming, multimedia systems, and UI/UX design.
      <br />
      <br />Now, as I step into the professional world, I’m excited to bring both my technical expertise and creativity to real-world projects. 
      While programming remains a core passion, I’m equally enthusiastic about taking on any technical-related tasks that allow me to learn, grow, and contribute. I am committed to continuous improvement and eager to be part of the ever-evolving tech and digital innovation industry.
      <br />
      <br />This is just the beginning of my journey, and I look forward to the opportunities ahead where I can make a meaningful impact. If there’s any opportunity, feel free to 
      <router-link to="/contact">contact me</router-link>.
      <br />

      <div style="margin-top:20px; margin-bottom:20px;">
        <a class="download-link" href="d/Pro-Resume.pdf" target="_blank"><i class="fa fa-download fa-lg fa-fw"></i> Download as PDF</a>
        <div style="clear:both"></div>
      </div>
    </div>
    <div class="photo">
      <img src="img/me-photo.jpg" alt="Photo of me" />
    </div>

    <div style="clear:both"></div>

    <div class="full-content">
      <h2>Work experience</h2>

      <h3>Mahkota Medical Centre (MMC)</h3>
      <h4>June 2019 - August 2019</h4>

      <div>Provided IT support across departments by troubleshooting and resolving hardware and software issues, ensuring smooth operation of devices.</div>

      <h3>Qudwah Technology</h3>
      <h4>October 2024 - March 2025</h4>

      <div>Managed daily social media content and marketing campaigns, created promotional videos, conducted customer outreach, maintained CRM data, and developed a Python automation tool to enhance data processing efficiency.</div>

      <h2>Skills</h2>

      <div class="skills-wrapper">

        <div class="skill-set">
          <h3>Programming Languages</h3>
          <div class="skills-grid">
          <SkillRate name="C++" />
          <SkillRate name="C#" />
          <SkillRate name="C" />
          <SkillRate name="Python" />
          <SkillRate name="HTML" />
          <SkillRate name="MySQL" />
          <SkillRate name="JavaScript" />
          <SkillRate name="phpMyAdmin" />
          </div>
        </div>

        <div class="skill-set">
          <h3>Technical Tools & Softwares</h3>
          <div class="skills-grid">
          <SkillRate name="Arduino" />
          <SkillRate name="Adobe Photoshop" />
          <SkillRate name="Adobe Illustrator" />
          <SkillRate name="Adobe Premiere Pro" />
          <SkillRate name="Adobe After Effects" />
          <SkillRate name="Blender" />
          <SkillRate name="Unreal Engine 5" />
          <SkillRate name="Unity" />
          <SkillRate name="Canva" />
          <SkillRate name="Capcut" />
          <SkillRate name="Capcut" />
          <SkillRate name="Microsoft Office Suite (Word, Excel, PowerPoint)" />
          </div>
        </div>

        <div class="skill-set">
          <h3>Soft Skills</h3>
          <div class="skills-grid">
          <SkillRate name="Adaptability" />
          <SkillRate name="Attention to Detail" />
          <SkillRate name="Communication" />
          <SkillRate name="Creativity" />
          <SkillRate name="Documentation" />
          <SkillRate name="Multitasking" />
          <SkillRate name="Project Management" />
          <SkillRate name="Problem-Solving" />
          <SkillRate name="Teamwork" />
          <SkillRate name="Team Leadership" />
          <SkillRate name="Time Management" />
          <SkillRate name="Technical Support" />
          <SkillRate name="Willingness to Learn" />
          <SkillRate name="Data Management & Reporting" />
          </div>
        </div>

      </div>
      <div style="clear:both" />

  
      <h2>Education</h2>

      <h3>[Diploma] Universiti Teknikal Malaysia Melaka (UTeM)</h3>
      <h4>Computer Science</h4>
      <div>Built a strong foundation in programming, web development, and database management, with design skills in Photoshop and full-stack experience using HTML, CSS, JavaScript, PHP, MySQL, and phpMyAdmin.</div>

      <h3>[Degree] Universiti Teknikal Malaysia Melaka (UTeM)</h3>
      <h4>Games Technology</h4>
      <div>Strong background in Game Technology with a focus on game development, multimedia systems, and UI/UX design. Experienced in building 2D and 3D games using Unity and Unreal Engine. Developed creative and technical skills in AI, animation, game management, and mechanics. Proficient in Blender, Adobe Creative Suite, and After Effects for game production. </div>

      <h2>Languages</h2>

      <h3>Malay</h3>
      <div>Native speaker</div>

      <h3>English</h3>
      <div>Proficient</div>

      <h3>Japanese</h3>
      <div>Basic</div>

      <h2>Hobby-Time-spending</h2>
      <div>

        <h3>Sports</h3>
        <div>I have explored a variety of sports over the years, especially during my student days. I tried wall climbing, kayaking, tennis, and more. I regularly played badminton, cycled, and enjoyed pétanque. </div>
        <br>
        <div>However, these days, I find myself drawn to hiking more than anything else. There is something incredibly grounding about being out on the trails, feeling as though I am becoming one with nature. The scenery is always breathtaking, and hiking has become my way of healing both mentally and physically, while also improving my overall health.</div>


      </div>
    </div>
  </div>
</template>

<script lang="ts">
import Vue from "vue";
import SkillRate from "@/components/SkillRate.vue";

export default Vue.extend({
  name: "Resume",
  components: {
    SkillRate,
  },
});
</script>

<style scoped>

.photo img {
  opacity: 0;
  transform: translateY(-30px) scale(0.95);
  animation: fadeSlideZoom 1s ease-out forwards;
}

@keyframes fadeSlideZoom {
  to {
    opacity: 1;
    transform: translateY(0) scale(1);
  }
}

.skills-wrapper {
  display: flex;
  justify-content: space-between;
  gap: 50px;
  flex-wrap: wrap; /* allow responsive stacking on small screens */
}

.skill-set {
  flex: 1;
  min-width: 300px;
}

.skills-grid {
  display: grid;
  grid-template-columns: repeat(2, 1fr); /* 2-column skills */
}

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


h2 {
  font-weight: 100;
  font-size: 2em;
  margin: 0px;
  padding: 0px;
  padding-top: 50px;
}
h3 {
  font-weight: 100;
  font-size: 1.6em;
  margin: 0px;
  padding: 0px;
  padding-top: 30px;
}
h4 {
  font-weight: 100;
  font-size: 1.3em;
  margin: 0px;
  padding: 0px;
  padding-top: 15px;
  font-style: italic;
}

.paragraph {
  max-width: 700px;
}

.download-link {
  float:left;
  margin-right: 50px;
}

.full-content div {
  max-width: 800px;
}

.skill-set h3 {
  padding-bottom: 10px;
}

.photo img {
  height: 300px;
  width: 300px;
}

.tech-stack {
  font-style: italic;
}

.photo {
  margin-top: 50px;
  text-align: center;
}

@media only screen and (min-width: 620px){
  .paragraph {
    float: left;
  }

  .photo {
    float: left;
    padding: 30px;
    padding-left: 80px;
  }

  .skill-set {
    float: left;
    padding-right: 60px; 
  }
}
</style>