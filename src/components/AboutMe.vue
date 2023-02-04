<template>
   <div>
   <!-- <img :src="imageSrc" width="100%" height="300"  style="position: absolute; z-index: 0.5; top: 60%; left: 15%;"/>--> 
    <h1 class="sui animated-text black white--text">
           I am a C++ and QT/QML software developer who loves to work in 
           innovative projects and needs of the society.  
    </h1>
    <h1 class="sui2 animated-text2 black white--text">
      I made a change in career from "Medicine" to Tech due to my interest in programming and technology 
      from a young age.
    </h1>

    <h1 class="sui3 animated-text3">
       
    </h1>

    <h1 class="sui4 animated-text">
       
    </h1>
  </div>


</template>
<script>
export default {
    
      
   data() {
    return {
            imageSrc: ''
    
           }
          }
        }

    


</script>
<style>
.sui {
   font-style: initial;
   font-weight: 500;
   font-family:'Franklin Gothic Medium', 'Arial Narrow', Arial, sans-serif;
   
  
   z-index: 1;
   
   color: rgb(255, 255, 255);

   
 
  position: absolute;
  left: 20%;
  top: 20%;
  width: 70%;
   
}

.animated-text {
 animation: write 4s steps(20, end) ;
 animation-play-state: running;

  
  animation-fill-mode:forwards;
}
@keyframes write {
   from { opacity:0}
   to{opacity:0.9 }
}

.sui2 {
   font-style: initial;
   font-weight: 500;
   font-family:'Franklin Gothic Medium', 'Arial Narrow', Arial, sans-serif;
   
  
   z-index: 1;
   
   color: rgb(255, 255, 255);

   
 
  position: absolute;
  left: 20%;
  top: 40%;
  width: 70%;
   
}
.animated-text2 {
 animation: write 6s steps(10, end) ;
 animation-play-state: running;

  
  animation-fill-mode:forwards;
}
@keyframes write {
   from { opacity:0}
   to{opacity:0.9 }
}


</style>