<template>
 
  <v-app >
    <v-app-bar
      app
      color="primary"
      dark
      class="appbar"
    >
      <div class="d-flex align-center">
        <v-img
          alt="Vuetify Logo"
          class="shrink mr-2"
          contain
          src="https://raw.githubusercontent.com/leodave/My-Certifications/main/photo_1.jpg"
          transition="scale-transition"
          width="40"
        />
        
        <v-btn   v-if=showMenu  x-large success @click="toggleToolbar" width="150">Menu</v-btn>
        
      </div>
      <v-spacer />
      <v-btn x-large success @click="homePage">Home-Page</v-btn>
      
      
     

      <v-spacer></v-spacer>

      <v-btn
        href="https://github.com/vuetifyjs/vuetify/releases/latest"
        target="_blank"
        text
      >
        <span class="mr-2">Latest Release</span>
        <v-icon>mdi-open-in-new</v-icon>
      </v-btn>
    </v-app-bar>
      
    <v-main>  
    
      <video class="bg-video" :src="require('@/assets/Binary - 847.mp4')" ref="videoPlayer" autoplay loop muted>
      
        
     </video> 
    
      <div class="content">
        <!--<div v-show="showInfo">
        <v-row>
      <v-col cols="4" class="info mt-15"><h1>suiiii</h1></v-col></v-row>
        </div>-->
    </div>
  
    
    
      <span v-show="btn">
        <v-card
         elevation="24"
         color="blue"
         height="600"
         width="200"
         outlined
         tile
         style="position: absolute; z-index: 1;"
         
        >
          <v-btn x-large success class="mt-5 ml-5" width="150" height="30" @click="menuButtons"><router-link to="/aboutme" class="text-decoration">About Me</router-link></v-btn>
          <v-btn x-large success class="mt-5 ml-5" width="150" height="35" @click="menuButtons"><router-link to="/education" class="text-decoration">Education & <br>Certifications</router-link></v-btn>
          <v-btn x-large success class="mt-5 ml-5" width="150" height="30" @click="menuButtons"><router-link to="/experience" class="text-decoration">Experience</router-link></v-btn>
          <v-btn x-large success class="mt-5 ml-5" width="150" height="30" @click="menuButtons"><router-link to="/projects" class="text-decoration">Projects</router-link></v-btn>
          <v-btn x-large success class="mt-5 ml-5" width="150" height="30" @click="menuButtons"><router-link to="/hobbies" class="text-decoration">Hobbies</router-link></v-btn>
          
          <v-btn x-large success class="mt-5 ml-5 white blue--text" width="150"  height="30" @click="menuButtons" href="https://www.linkedin.com/in/dawit-elias/"  target="_blank" text>LinkedIN</v-btn>
          <v-btn x-large success class="mt-5 ml-5 white blue--text" width="150"  height="30" @click="menuButtons" href="https://github.com/leodave"  target="_blank" text>GitHub</v-btn>
          <v-btn x-large success class="mt-5 ml-5 white blue--text" width="150"  height="30" @click="menuButtons" href="https://www.linkedin.com/in/dawit-elias/"  target="_blank" text>CV</v-btn>

      </v-card>
      
    
  
      
     <router-view/> 
    </span>
    <span v-show="!btn">
      <router-view/>
    </span>
    </v-main>
  </v-app>

</template>

<script>

export default {
  name: 'App',
  mounted() {
    this.$refs.videoPlayer.volume = 0
  },

  data() {
    return {
      btn: true,
      showMenu:true,
    }
  },
  methods: {
   async toggleToolbar() {
      this.btn= !this.btn;
      
      
    },
    async menuButtons() {
      //this.showMenu=false;
      this.btn= !this.btn;
    },
    async homePage() {
      
      this.$router.push('/')
      //this.showMenu=!this.showMenu;
    }
  },
};
</script>
<style>


.appbar {
  height: 200px;
}
.bg-video {
  position: absolute;
  top: 0;
  left: 0;
  min-width: 100%;
  height: 1500px;
  overflow: hidden;
}


.bg-video video {
  position: absolute;
  top: 1500px;
  left: 100%;
  min-width: 100%;
  min-height: 300%;
  width: auto;
  height: 500px;
  z-index: -100;
  transform: translateX(-50%) translateY(-50%);
}


.content {
  position: relative;
  z-index: 1;
}
.text-decoration {
  text-decoration: none;
}
.bot {
  color: white;
}

</style>
