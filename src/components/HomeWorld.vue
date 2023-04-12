<template>
  <v-container class="cont ml-15 mb-15">
    <div class="ml-15">
      <div>
        <span class="back">
          <v-spacer />
          <span>D</span>
          <span>A</span>
          <span>W</span>
          <span>I</span>
          <span>T</span>
          <span></span>
          <span>E</span>
          <span>L</span>
          <span>I</span>
          <span>A</span>
          <span>S</span>
        </span>
        <img
          class="circle-frame1"
          src="@/assets/photo_1.jpeg"
          width="200"
          height="300"
          style="position: absolute; z-index: 0.5; top: 65%; left: 40%"
          @mouseover="hover1 = true"
          @mouseleave="hover1 = false"
          :style="{ transform: hover1 ? 'scale(1.2)' : 'scale(1)' }"
        />
        <router-link to="/education" class="text-decoration">
          <img
            class="circle-frame"
            src="@/assets/education.jpeg"
            width="400"
            height="300"
            style="position: absolute; z-index: 0.5; top: 115%; left: 20%"
            @mouseover="hover = true"
            @mouseleave="hover = false"
            :style="{ transform: hover ? 'scale(1.2)' : 'scale(1)' }"
          />
        </router-link>
        <router-link to="/experience" class="text-decoration">
          <img
            class="circle-frame"
            src="@/assets/experience.jpeg"
            width="400"
            height="300"
            style="position: absolute; z-index: 0.5; top: 115%; left: 60%"
            @mouseover="hover2 = true"
            @mouseleave="hover2 = false"
            :style="{ transform: hover2 ? 'scale(1.2)' : 'scale(1)' }"
          />
        </router-link>
        <router-link to="/hobbies" class="text-decoration">
          <img
            class="circle-frame"
            src="@/assets/hobbie.jpeg"
            width="400"
            height="300"
            style="position: absolute; z-index: 0.5; top: 180%; left: 40%"
            @mouseover="hover3 = true"
            @mouseleave="hover3 = false"
            :style="{ transform: hover3 ? 'scale(1.2)' : 'scale(1)' }"
          />
        </router-link>
        <a
          href="https://github.com/leodave/My-Certifications/blob/main/updated-dave.pdf"
          target="_blank"
        >
          <img
            class="circle-frame"
            src="@/assets/cv.jpeg"
            width="400"
            height="300"
            style="position: absolute; z-index: 0.5; top: 245%; left: 20%"
            @mouseover="hover4 = true"
            @mouseleave="hover4 = false"
            :style="{ transform: hover4 ? 'scale(1.2)' : 'scale(1)' }"
          />
        </a>
        <a href="https://github.com/leodave" target="_blank">
          <img
            class="circle-frame"
            src="@/assets/github.png"
            width="400"
            height="300"
            style="position: absolute; z-index: 0.5; top: 245%; left: 60%"
            @mouseover="hover5 = true"
            @mouseleave="hover5 = false"
            :style="{ transform: hover5 ? 'scale(1.2)' : 'scale(1)' }"
          />
        </a>
        <div class="cv"></div>
        <div class="cv"></div>
      </div>
    </div>
  </v-container>
</template>

<script>
export default {
  name: "HomeWorld",

  data() {
    return {
      hover: false,
      hover2: false,
      hover3: false,
      hover4: false,
      hover5: false,
      imageSrc: "@/assets/education.jpeg",
      imageSrc2: "@/assets/experience.jpeg",
      imageSrc3: "@/assets/hobbie.jpeg",
      imageSrc4: "@/assets/cv.jpeg",
      imageSrc5: "@/assets/github.png",
      imageSrc1: "@/assets/photo_1.jpeg",
    };
  },
};
</script>
<style>
.info {
  color: aqua;
}
.cont {
  background: transparent;
}

@import url(https://fonts.googleapis.com/css?family=Roboto:300);
html {
  height: 90%;
}

body {
  background: #3f485b;

  height: 90%;
}
.back {
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  font-family: "Roboto";
}
.back span {
  font-size: 3em;
  color: #f2c640;
  background: #262b37;
  display: table-cell;
  box-shadow: inset 0 0 5px rgba(0, 0, 0, 0.3), 0 5px 0 #ccc;
  padding: 0 20px;
  line-height: 100px;
  animation: jumb 2s infinite;
}
@keyframes jumb {
  0% {
    transform: translateY(0px);
  }
  50% {
    transform: translateY(-50px);
    box-shadow: 0 15px 0 rgb(242, 198, 64);
  }
  100% {
    transform: translateY(0px);
  }
}
.back span:nth-child(1) {
  animation-delay: 0s;
}
.back span:nth-child(2) {
  animation-delay: 0.1s;
}
.back span:nth-child(3) {
  animation-delay: 0.2s;
}
.back span:nth-child(4) {
  animation-delay: 0.3s;
}
.back span:nth-child(5) {
  animation-delay: 0.4s;
}
.back span:nth-child(6) {
  animation-delay: 0.5s;
}
.back span:nth-child(7) {
  animation-delay: 0.6s;
}
.back span:nth-child(8) {
  animation-delay: 0.5s;
}
.back span:nth-child(9) {
  animation-delay: 0.8s;
}
.back span:nth-child(10) {
  animation-delay: 0.9s;
}
.back span:nth-child(11) {
  animation-delay: 0.1s;
}
.back span:nth-child(12) {
  animation-delay: 0.11s;
}
.circle-frame {
  border-radius: 50%;
  border: 5px solid white;
  overflow: hidden;
  width: 400px;
  height: 300px;
}

.circle-frame img {
  width: 100%;
  height: 100%;
  object-fit: cover;
}
.circle-frame1 {
  border-radius: 50%;
  border: 5px solid white;
  overflow: hidden;
  width: 300px;
  height: 300px;
}

.circle-frame1 img {
  width: 100%;
  height: 100%;
  object-fit: cover;
}
</style>
