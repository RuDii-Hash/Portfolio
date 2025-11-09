<template>
  <div>
    <h1>Resume</h1>

    <div class="paragraph">
      I'm <strong>Zohaib Maqsood</strong>, passionate game developer currently based in Debrecen, Hungary.
      <br />After graduating with a degree in Software Engineering in 2024, I worked as a Full Stack Developer at Stackwise for one year before beginning my master’s studies.
      <br /> I also worked as a freelance game developer, completing several Unity projects that helped me gain valuable experience.
      <br />I love teamwork, but I can also go in solo depending on the projects requirements.
      <br />
      <br />I am currently pursuing a Master’s degree in Computer Science Engineering at the University of Debrecen. I’m planning to apply for a Game Development program because I want to specialize and build a strong career in this gaming industry. 
      <router-link to="/contact"></router-link>
      <br />
      <br />Besides development, I love playing video games , and traveling across the world.

      <div style="margin-top:20px; margin-bottom:20px;">
        <a class="download-link" href="d/resume-en.pdf" target="_blank"><i class="fa fa-download fa-lg fa-fw"></i> Download my CV</a>
        <a class="download-link" href="d/cv-fr.pdf" target="_blank"><i class="fa  fa-lg fa-fw"></i> </a>
        <div style="clear:both"></div>
      </div>
    </div>
    <div class="photo">
      <img src="img/resume-photo.png" alt="Photo of John" />
    </div>

    <div style="clear:both"></div>

    <div class="full-content">
      <h2>Work experience</h2>

      <h3>Software Developer - Stackwise</h3>
      <h4>2024-2025</h4>

      <div>- Designed and developed mobile and web applications.</div>
      <div>- Integrated APIs, managed databases, and optimized backend systems.</div>
      <div>- Worked with Agile teams, performance testing, code reviews.</div>
       <div>- Created modern, responsive UI/UX designs.</div>



      <h2>Skills</h2>

      <div class="skill-set">
        <h3>Languages</h3>
        <SkillRate name="Python" :rate="5" />
        <SkillRate name="C#" :rate="5" />
        <SkillRate name="C++" :rate="5" />
         <SkillRate name="Javascript" :rate="5" />

      </div>

      <div class="skill-set">
        <h3>Gamedev</h3>
        <SkillRate name="Unity" :rate="5" />
        <SkillRate name="Unreal" :rate="5" />
        <SkillRate name="Blender" :rate="5" />
        <SkillRate name="Photoshop" :rate="5" />
      </div>

          <div class="skill-set">
        <h3>Tools & Frameworks</h3>
        <SkillRate name="Visual Studio" :rate="5" />
        <SkillRate name="Matlab" :rate="5" />
        <SkillRate name="Pycharm" :rate="5" />
        <SkillRate name=".NET" :rate="5" />
      </div>

      <div style="clear:both" />

      <h2>Education</h2>

      <h3>Debrecn University - 2025</h3>
      <h4>Computer Science Engineering (Masters)</h4>
      <div>Specialty in Embedded systems & information technology</div>

      <h3>Comsats University - 2024</h3>
      <h4>Software Engineering (Bachelor)</h4>
      <div>Specialty in Software development & Designing</div>

      <h3>Scholar Science Collage - 2020</h3>
      <h4>Genral Science (Intermediate)</h4>
      <div>Specialty in genral science & Mathematics</div>

      <h2>Languages</h2>

      <h3>English</h3>
      <div>Fluent</div>

      <h3>German</h3>
      <div> Basic Knowledge</div>


      <h2>Besides...</h2>
      <div>
        <h3>Video games</h3>
        <div>I enjoy playing video games and have participated in many competitive gaming events..</div>

        <h3>Sports</h3>
        <div>I’m passionate about sports, especially football and cricket..</div>


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
