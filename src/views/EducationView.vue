<template>
<div>
        <img :src="imageSrc" width="100" height="100"  style="position: absolute; z-index: 0.5; top: 5%; left: 10%;"/>
        <h1 class="qt black white--text"> QT which is also called "QML" due to its additional feauture, is an upcoming 
            Software development technology that sits on C++. 
            Additionally it can integrate javascript and phyton. 
        </h1>
        <h1 class="qt2 black white--text"> It is mainly used in the production of desktop and mobile software that can be accessible
            on mac,windows and linux, whereas for the mobile applications both on IOS and Android phones. 
        </h1>
        <a :href="linkUrl" target="_blank">
        <img :src="imageSrc2" width="400" height="300"  style="position: absolute; z-index: 0.5; top: 50%; left: 35%;"
                                                         @mouseover="hover = true" @mouseleave="hover = false"
                                                        :style="{ transform: hover ? 'scale(1.2)' : 'scale(1)' }"/>
         </a> 
         <a :href="linkUrl2" target="_blank">                                              
        <img :src="imageSrc3" width="330" height="250"  style="position: absolute; z-index: 0.5; top: 75%; left: 70%;"
                                                        @mouseover="hover2 = true" @mouseleave="hover2 = false"
                                                        :style="{ transform: hover2 ? 'scale(1.2)' : 'scale(1)' }"/>
        </a>
        <a :href="linkUrl3" target="_blank">                                                 
        <img :src="imageSrc4" width="330" height="250"  style="position: absolute; z-index: 0.5; top: 75%; left: 5%;"
                                                        @mouseover="hover3 = true" @mouseleave="hover3 = false"
                                                        :style="{ transform: hover3 ? 'scale(1.2)' : 'scale(1)' }"/>
        </a>
        <div class="full-width-line"  style="position: absolute; z-index: 0.5; top: 135%; left: 10%;"></div>
        <img :src="imageSrc5" width="200" height="180"  style="position: absolute; z-index: 0.5; top: 150%; left: 8%;"/>
        <h1 class="java black white--text"> I have been using Java with spring Boot as a backend for quite some time now. 
            My fullstack projects done with my great classmates was using java as its back end.
        </h1>
        <h1 class="java2 black white--text"> our project "<a :href="linkUrl4" target="_blank">League Pong</a>" was an 
            application that help organize leagues of ping pong (Table Tennis) through out the city of Barcelona.
        </h1>
        <a :href="linkUrl5" target="_blank">  
        <img :src="imageSrc6" width="400" height="450"  style="position: absolute; z-index: 0.5; top: 150%; left: 60%;"
                                                        @mouseover="hover4 = true" @mouseleave="hover4 = false"
                                                        :style="{ transform: hover4 ? 'scale(1.2)' : 'scale(1)' }"/>
        </a>
        <div class="full-width-line2"  style="position: absolute; z-index: 0.5; top: 246%; left: 10%;"></div>
        <img :src="imageSrc7" width="300" height="80"  style="position: absolute; z-index: 0.5; top: 258%; left: 40%;"/>
        

</div>
</template>
<script>
export default {
  name: 'EducationView',

  data() {
    return {
            imageSrc: 'https://raw.githubusercontent.com/leodave/My-Certifications/main/qtimg.png',
            imageSrc2: 'https://raw.githubusercontent.com/leodave/My-Certifications/main/Screenshot%202023-02-04%20at%201.30.10%20AM.png',
            imageSrc3: 'https://raw.githubusercontent.com/leodave/My-Certifications/main/Screenshot%202023-02-04%20at%201.29.53%20AM.png',
            imageSrc4: 'https://raw.githubusercontent.com/leodave/My-Certifications/main/Screenshot%202023-02-04%20at%201.29.30%20AM.png',

            hover: false,
            hover2: false,
            hover3: false,
            linkUrl: 'https://github.com/leodave/My-Certifications/blob/main/qt-qml-ceritificate%20dawit.pdf',
            linkUrl2:'https://github.com/leodave/My-Certifications/blob/main/dawit-Agil-certificate.pdf',
            linkUrl3: 'https://github.com/leodave/My-Certifications/blob/main/Dawit-Itil-Certificate.pdf',

            imageSrc5:'https://w0.peakpx.com/wallpaper/389/1004/HD-wallpaper-java-logo-white-silk-texture-java-emblem-programming-language-java-silk-background.jpg',
            linkUrl4: 'https://github.com/leodave/Complete-Full-Stack-Website-Projects/tree/main/LeaguePong-App-For_Organizing-PingPong-Lagues',
            imageSrc6: 'https://raw.githubusercontent.com/leodave/My-Certifications/main/Screenshot%202023-02-04%20at%201.33.09%20AM.png',
            linkUrl5: 'https://github.com/leodave/My-Certifications/blob/main/java-fundacion-certificate.pdf',
            hover4: false,
            imageSrc7:'https://raw.githubusercontent.com/leodave/My-Certifications/main/epi.png'
           }
          }
        
}
</script>
<style>
.qt{
   font-style: initial;
   font-weight: 50;
   font-size:x-large;
   font-family:'Franklin Gothic Medium', 'Arial Narrow', Arial, sans-serif;

  position: absolute;
  left: 20%;
  top: 5%;
  width: 80%;
}
.qt2{
   font-style: initial;
   font-weight: 50;
   font-size:x-large;
   font-family:'Franklin Gothic Medium', 'Arial Narrow', Arial, sans-serif;

  position: absolute;
  left: 20%;
  top: 25%;
  width: 80%;
}
.java{
   font-style: initial;
   font-weight: 10;
   font-size:x-large;
   font-family:'Franklin Gothic Medium', 'Arial Narrow', Arial, sans-serif;

   

  position: absolute;
  left: 25%;
  top: 150%;
  width: 30%;
}
.java2{
   font-style: initial;
   font-weight: 10;
   font-size:x-large;
   font-family:'Franklin Gothic Medium', 'Arial Narrow', Arial, sans-serif;

   

  position: absolute;
  left: 25%;
  top: 200%;
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
</style>