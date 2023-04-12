<template>
  <div>
    <video
      class="bg-videoedu"
      :src="require('@/assets/Chain - 25380.mp4')"
      ref="videoPlayer"
      autoplay
      loop
      muted
    ></video>
    <img
      src="@/assets/qtimg.png"
      width="100"
      height="100"
      style="position: absolute; z-index: 0.5; top: 5%; left: 10%"
    />
    <h1 class="qt black white--text">
      QT which is also called "QML" due to its additional feauture, is an
      upcoming Software development technology that sits on C++. Additionally it
      can integrate javascript and phyton.
    </h1>
    <h1 class="qt2 black white--text">
      It is mainly used in the production of desktop and mobile software that
      can be accessible on mac,windows and linux, whereas for the mobile
      applications both on IOS and Android phones.
    </h1>
    <a :href="linkUrl" target="_blank">
      <img
        src="@/assets/qmlcertification.png"
        width="400"
        height="300"
        style="position: absolute; z-index: 0.5; top: 50%; left: 35%"
        @mouseover="hover = true"
        @mouseleave="hover = false"
        :style="{ transform: hover ? 'scale(1.2)' : 'scale(1)' }"
      />
    </a>
    <a :href="linkUrl2" target="_blank">
      <img
        src="@/assets/agil-certification.png"
        width="330"
        height="250"
        style="position: absolute; z-index: 0.5; top: 75%; left: 70%"
        @mouseover="hover2 = true"
        @mouseleave="hover2 = false"
        :style="{ transform: hover2 ? 'scale(1.2)' : 'scale(1)' }"
      />
    </a>
    <a :href="linkUrl3" target="_blank">
      <img
        src="@/assets/itil-certification.png"
        width="330"
        height="250"
        style="position: absolute; z-index: 0.5; top: 75%; left: 5%"
        @mouseover="hover3 = true"
        @mouseleave="hover3 = false"
        :style="{ transform: hover3 ? 'scale(1.2)' : 'scale(1)' }"
      />
    </a>
    <div
      class="full-width-line"
      style="position: absolute; z-index: 0.5; top: 135%; left: 10%"
    ></div>
    <img
      src="@/assets/javaaa.jpeg"
      width="200"
      height="250"
      style="position: absolute; z-index: 0.5; top: 150%; left: 8%"
    />
    <h1 class="java black white--text">
      I have been using Java with spring Boot as a backend for quite some time
      now. My fullstack projects done with my great classmates was using java as
      its back end.
    </h1>
    <h1 class="java2 black white--text">
      our project "
      <a :href="linkUrl4" target="_blank">League Pong</a>
      " was an application that help organize leagues of ping pong (Table
      Tennis) through out the city of Barcelona.
    </h1>
    <a :href="linkUrl5" target="_blank">
      <img
        src="@/assets/java-fundacion-certification.png"
        width="400"
        height="450"
        style="position: absolute; z-index: 0.5; top: 150%; left: 60%"
        @mouseover="hover4 = true"
        @mouseleave="hover4 = false"
        :style="{ transform: hover4 ? 'scale(1.2)' : 'scale(1)' }"
      />
    </a>
    <div
      class="full-width-line2"
      style="position: absolute; z-index: 0.5; top: 246%; left: 10%"
    ></div>
    <img
      src="@/assets/epi.png"
      width="400"
      height="70"
      style="position: absolute; z-index: 20; top: 258%; left: 35%"
    />
    <img
      src="@/assets/epi2.jpeg"
      width="1150"
      height="600"
      style="position: absolute; z-index: 0; top: 270%; left: 10%"
    />
    <h1 class="epi grey black--text">
      Epitech was the University I took my first formal programming class, even
      tho I had prior begginner knowledge from youtube. we spent 9 hours
      everyday for almost a year during this intensive and vast program held by
      the university.
    </h1>
    <h1 class="epi2 grey black--text">
      I had a very interesting and intense time during my course with a self
      teaching methedology with the proffesor present for your guidance. Besides
      the course, It helped me how to learn, search and solve my problems by
      myself. I have listed below some of the technologies covered during this
      program.
    </h1>
    <img
      src="@/assets/git.png"
      width="120"
      height="120"
      style="position: absolute; z-index: 0; top: 365%; left: 10%"
    />
    <img
      src="@/assets/htmlcss.png"
      width="120"
      height="120"
      style="position: absolute; z-index: 0; top: 365%; left: 20%"
    />
    <img
      src="@/assets/js.png"
      width="120"
      height="120"
      style="position: absolute; z-index: 0; top: 365%; left: 30%"
    />
    <img
      src="@/assets/expo-react.png"
      width="120"
      height="120"
      style="position: absolute; z-index: 0; top: 365%; left: 40%"
    />
    <img
      src="@/assets/nest.png"
      width="120"
      height="120"
      style="position: absolute; z-index: 0; top: 365%; left: 50%"
    />
    <img
      src="@/assets/node-express.png"
      width="120"
      height="120"
      style="position: absolute; z-index: 0; top: 365%; left: 60%"
    />
    <img
      src="@/assets/sql.png"
      width="120"
      height="120"
      style="position: absolute; z-index: 0; top: 365%; left: 70%"
    />
    <img
      src="@/assets/wordpress.png"
      width="120"
      height="120"
      style="position: absolute; z-index: 0; top: 365%; left: 80%"
    />
    <img
      src="@/assets/mongo.png"
      width="150"
      height="80"
      style="position: absolute; z-index: 0; top: 385%; left: 35%"
    />
    <img
      src="@/assets/vue.png"
      width="150"
      height="80"
      style="position: absolute; z-index: 0; top: 385%; left: 55%"
    />
    <a :href="linkUrl6" target="_blank">
      <img
        src="@/assets/epitech-certification.png"
        width="800"
        height="500"
        style="position: absolute; z-index: 0; top: 400%; left: 20%"
        @mouseover="hover5 = true"
        @mouseleave="hover5 = false"
        :style="{ transform: hover5 ? 'scale(1.2)' : 'scale(1)' }"
      />
    </a>
    <div
      class="full-width-line3"
      style="position: absolute; z-index: 0.5; top: 480%; left: 10%"
    ></div>
    <img
      src="@/assets/amc.png"
      width="400"
      height="100"
      style="position: absolute; z-index: 0; top: 485%; left: 35%"
    />
    <a :href="linkUrl17" target="_blank">
      <img
        src="@/assets/amc-grades.png"
        width="400"
        height="450"
        style="position: absolute; z-index: 1; top: 510%; left: 20%"
        @mouseover="hover6 = true"
        @mouseleave="hover6 = false"
        :style="{ transform: hover6 ? 'scale(1.5)' : 'scale(1)' }"
      />
    </a>
    <h1 class="africa black white--text">
      I first joined a medical University in Ethiopia due to family pressure as
      my mom is also an Oncologisy. But not for long as I relocated to spain and
      started my programming journey in Barcelona.
    </h1>
    <h1 class="africa2 black white--text">
      During my stay of 2 years, I had good grades and and also discovered
      health was an interesting and lovable area of study. Well later on I
      withdrew and went to spain as soon as I got the opportunity to pursue what
      i want.
    </h1>
    <div
      class="full-width-line4"
      style="position: absolute; z-index: 0.5; top: 580%; left: 10%"
    ></div>
  </div>
</template>
<script>
export default {
  name: "EducationView",

  data() {
    return {
      hover: false,
      hover2: false,
      hover3: false,
      linkUrl:
        "https://github.com/leodave/My-Certifications/blob/main/qt-qml-ceritificate%20dawit.pdf",
      linkUrl2:
        "https://github.com/leodave/My-Certifications/blob/main/dawit-Agil-certificate.pdf",
      linkUrl3:
        "https://github.com/leodave/My-Certifications/blob/main/Dawit-Itil-Certificate.pdf",

      linkUrl4:
        "https://github.com/leodave/Complete-Full-Stack-Website-Projects/tree/main/LeaguePong-App-For_Organizing-PingPong-Lagues",

      linkUrl5:
        "https://github.com/leodave/My-Certifications/blob/main/java-fundacion-certificate.pdf",
      hover4: false,

      linkUrl6:
        "https://github.com/leodave/My-Certifications/blob/main/epitech-certificate.pdf",
      hover5: false,

      linkUrl17:
        "https://github.com/leodave/My-Certifications/blob/main/Africa%20md%20grades.pdf",
      hover6: false,
    };
  },
};
</script>
<style>
.qt {
  font-style: initial;
  font-weight: 50;
  font-size: x-large;
  font-family: "Franklin Gothic Medium", "Arial Narrow", Arial, sans-serif;

  position: absolute;
  left: 20%;
  top: 5%;
  width: 80%;
}
.qt2 {
  font-style: initial;
  font-weight: 50;
  font-size: x-large;
  font-family: "Franklin Gothic Medium", "Arial Narrow", Arial, sans-serif;

  position: absolute;
  left: 20%;
  top: 25%;
  width: 80%;
}
.java {
  font-style: initial;
  font-weight: 10;
  font-size: x-large;
  font-family: "Franklin Gothic Medium", "Arial Narrow", Arial, sans-serif;

  position: absolute;
  left: 25%;
  top: 150%;
  width: 30%;
}
.java2 {
  font-style: initial;
  font-weight: 10;
  font-size: x-large;
  font-family: "Franklin Gothic Medium", "Arial Narrow", Arial, sans-serif;

  position: absolute;
  left: 25%;
  top: 190%;
  width: 30%;
}
.full-width-line {
  width: 80%;
  height: 1px;
  border-bottom: 20px solid rgb(240, 233, 233);
}
.full-width-line2 {
  width: 80%;
  height: 1px;
  border-bottom: 20px solid rgb(240, 233, 233);
}
.epi {
  font-style: inherit;
  font-weight: 20;
  font-size: x-large;
  font-family: "Franklin Gothic Medium", "Arial Narrow", Arial, sans-serif;

  position: absolute;
  left: 22%;
  top: 305%;
  width: 40%;
}
.epi2 {
  font-style: inherit;
  font-weight: 20;
  font-size: x-large;
  font-family: "Franklin Gothic Medium", "Arial Narrow", Arial, sans-serif;

  position: absolute;
  left: 22%;
  top: 331%;
  width: 40%;
}
.full-width-line3 {
  width: 80%;
  height: 1px;
  border-bottom: 20px solid rgb(240, 233, 233);
}
.africa {
  font-style: inherit;
  font-weight: 20;
  font-size: x-large;
  font-family: "Franklin Gothic Medium", "Arial Narrow", Arial, sans-serif;

  position: absolute;
  left: 50%;
  top: 510%;
  width: 45%;
}
.africa2 {
  font-style: inherit;
  font-weight: 20;
  font-size: x-large;
  font-family: "Franklin Gothic Medium", "Arial Narrow", Arial, sans-serif;

  position: absolute;
  left: 50%;
  top: 550%;
  width: 45%;
}
.full-width-line4 {
  width: 80%;
  height: 1px;
  border-bottom: 20px solid rgb(240, 233, 233);
}
.bg-videoedu {
  position: absolute;
  top: 0;
  left: 0;
  min-width: 100%;
  height: 620%;
  overflow: hidden;
}

.bg-videoedu video {
  position: absolute;
  top: 620%;
  left: 300%;
  min-width: 100%;
  min-height: 300%;
  width: auto;
  height: 500px;
  z-index: -100;
  transform: translateX(-50%) translateY(-50%);
}
</style>
