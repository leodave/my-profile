<template>
  <v-app>
    <v-app-bar app color="primary" dark class="appbar">
      <div class="d-flex align-center">
        <v-img
          alt="Vuetify Logo"
          class="shrink mr-2"
          contain
          src="@/assets/photo_1.jpeg"
          transition="scale-transition"
          width="40"
        />

        <v-btn
          v-if="showMenu"
          x-large
          success
          @click="toggleToolbar"
          width="150"
        >
          Menu
        </v-btn>
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
      <video
        class="bg-video"
        :src="require('@/assets/Chain - 25380.mp4')"
        ref="videoPlayer"
        autoplay
        loop
        muted
      ></video>

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
          height="420"
          width="200"
          outlined
          tile
          style="position: absolute; z-index: 1"
        >
          <!--<v-btn
            x-large
            success
            class="mt-5 ml-5"
            width="150"
            height="30"
            @click="menuButtons"
          >
            <router-link to="/aboutme" class="text-decoration">
              About Me
            </router-link>
          </v-btn>
        -->
          <v-btn
            x-large
            success
            class="mt-5 ml-5"
            width="150"
            height="35"
            @click="menuButtons"
          >
            <router-link to="/education" class="text-decoration">
              Education &
              <br />
              Certifications
            </router-link>
          </v-btn>
          <v-btn
            x-large
            success
            class="mt-5 ml-5"
            width="150"
            height="35"
            @click="menuButtons"
          >
            <router-link to="/experience" class="text-decoration">
              Experience &
              <br />
              Projects
            </router-link>
          </v-btn>
          <!--
          <v-btn
            x-large
            success
            class="mt-5 ml-5"
            width="150"
            height="30"
            @click="menuButtons"
          >
            <router-link to="/projects" class="text-decoration">
              Projects
            </router-link>
          </v-btn>-->

          <v-btn
            x-large
            success
            class="mt-5 ml-5 white blue--text"
            width="150"
            height="30"
            @click="menuButtons"
            href="https://www.linkedin.com/in/dawit-elias/"
            target="_blank"
            text
          >
            LinkedIN
          </v-btn>
          <v-btn
            x-large
            success
            class="mt-5 ml-5 white blue--text"
            width="150"
            height="30"
            @click="menuButtons"
            href="https://github.com/leodave"
            target="_blank"
            text
          >
            GitHub
          </v-btn>
          <v-btn
            x-large
            success
            class="mt-5 ml-5 white blue--text"
            width="150"
            height="30"
            @click="menuButtons"
            href="https://docs.google.com/document/d/1X-29FrbdgjlogSnUXZC605zlosmbaKq4tKx36oCSJww/edit"
            target="_blank"
            text
          >
            CV
          </v-btn>
          <v-btn
            x-large
            success
            class="mt-5 ml-5"
            width="150"
            height="30"
            @click="menuButtons"
          >
            <router-link to="/hobbies" class="text-decoration">
              Hobbies
            </router-link>
          </v-btn>
          <v-card
            class="mt-5 ml-5 mr-6 white blue--text"
            style="font-size: 18px"
          >
            (+34)722-522-442
          </v-card>
          <v-card
            class="mt-5 ml-5 mr-6 white blue--text"
            style="font-size: 13px"
          >
            dawitelias735@gmail.com
          </v-card>
        </v-card>

        <router-view />
      </span>
      <span v-show="!btn">
        <router-view />
      </span>
    </v-main>
  </v-app>
</template>

<script>
export default {
  name: "App",
  mounted() {
    this.$refs.videoPlayer.volume = 0;
  },

  data() {
    return {
      btn: true,
      showMenu: true,
    };
  },
  methods: {
    async toggleToolbar() {
      this.btn = !this.btn;
      window.scrollTo({ top: 0, behavior: "smooth" });
    },
    async menuButtons() {
      //this.showMenu=false;
      this.btn = !this.btn;
    },
    async homePage() {
      this.$router.push("/");
      //this.showMenu=!this.showMenu;
    },
  },
};
</script>
<style>
.appbar {
  height: 200px;
  z-index: 100;
}
.bg-video {
  position: absolute;
  top: 0;
  left: 0;
  min-width: 100%;
  height: 550%;
  overflow: hidden;
}

.bg-video video {
  position: absolute;
  top: 300%;
  left: 300%;
  min-width: 100%;
  min-height: 510%;
  width: auto;
  height: 550px;
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
