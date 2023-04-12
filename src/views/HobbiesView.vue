<template>
  <div>
    <h1 class="football white--text">
      Football has always been my sport from a young age. always loved and
      played the game with my friends and teammates in amateur leagues. i have
      put below some video of mine for you to enjoy a little!!!!!
      &nbsp;&nbsp;&nbsp;
      <h1>Press Video to Play!!!</h1>
    </h1>

    <div>
      <button @click="playvid">
        <video
          class="bg-videoplayer"
          :src="require('@/assets/david-video.mp4')"
          ref="videoPlayer"
          loop
        ></video>
      </button>
    </div>
  </div>
</template>
<script>
export default {
  name: "HobbiesView",
  data() {
    return {
      playing: true,
    };
  },
  onmounted() {
    this.$refs.videoPlayer.play();
  },

  methods: {
    playvid() {
      if (this.$refs.videoPlayer.paused) {
        this.$refs.videoPlayer.play();
        console.log("plaay");
      } else {
        this.$refs.videoPlayer.pause();
      }
    },
  },
};
</script>
<style>
.bg-videoplayer {
  position: absolute;
  top: 30%;
  left: 0;
  min-width: 100%;
  height: 80%;
  overflow: hidden;
}

.bg-videoplayer video {
  position: absolute;
  top: 80%;
  left: 100%;
  min-width: 100%;
  min-height: 300%;
  width: auto;
  height: 500px;
  z-index: -100;
  transform: translateX(-50%) translateY(-50%);
}
.football {
  font-style: inherit;
  font-weight: 25;
  font-size: x-large;
  font-family: "Franklin Gothic Medium", "Arial Narrow", Arial, sans-serif;

  position: absolute;
  left: 10%;
  top: 10%;
  width: 85%;
}
</style>
