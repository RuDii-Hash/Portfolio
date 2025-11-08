<template>
  <div style="margin-bottom: 80px;">
    <h1>Hello!</h1>

    <div class="paragraph">
      <div>
        I'm <strong>Zohaib Maqsood</strong>,  A Computer Science student and a part-time game developer with one year of experience as a Full Stack Developer. <br/>
        I’m passionate about game development and love designing and building games using the Unity Engine.
      </div>

      <div style="margin-top: 20px;">I've worked on various <router-link to="/game-projects">games</router-link> (either as a freelancer, to showcase my capabilities using Unity & unreal engine) <router-link to="/other-projects"></router-link>, and i also love developing mobile Applications <router-link to="/resume"></router-link> as well.</div>

      <div style="margin-top: 40px;">I'm <strong>applying for masters program   </strong> in game development, to echance my skills so i can I can pursue a career in the game industry. You can reach me at <a href="mailto:zohaib.maqsood991@gmail.com">zohaib.maqsood991@gmail.com</a>  <router-link to="/contact"></router-link>.</div>
    </div>

    <div class="photo">
      <img src="img/avatar.png" alt="Avatar of John" /> 
    </div>

    <div style="clear:both"></div>

  </div>
</template>

<style scoped>
.paragraph {
  max-width: 700px;
  margin-bottom: 20px;
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
    padding: 10px;
    padding-left: 80px;
  }
}

</style>