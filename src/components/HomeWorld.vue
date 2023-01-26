<template>
  <v-container class = "cont ml-15 mb-15">
  
   <div class="ml-15">
    <div>
    <span class="back">
<v-spacer/><span>D</span><span>A</span><span>W</span><span>I</span><span>T</span><span> </span>
  <span>E</span><span>L</span><span>I</span><span>A</span><span>S</span>

</span>
</div>
  
   </div>
  </v-container>
</template>

<script>
  export default {
    name: 'HomeWorld',

  }
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
      height:90%;
  }

  body {
     background:#3F485B;
   
     
     height:90%;
  }
  .back {
    position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%); 
    font-family:"Roboto";
  }
  .back span {
    font-size:3em;
    color:#F2C640;
    background:#262B37;
    display:table-cell;
    box-shadow:inset 0 0 5px rgba(0,0,0,0.3), 0 5px 0 #ccc;
    padding: 0 15px;
    line-height: 100px;
    animation:jumb 2s infinite;
  }
  @keyframes jumb {
    0% {
      transform:translateY(0px)
    }
    50% {
      transform:translateY(-50px);
      box-shadow:0 15px 0 rgb(242, 198, 64);
    }
    100% {
      transform:translateY(0px) 
    }
  }
  .back span:nth-child(1) {
    animation-delay:0s;
  }
  .back span:nth-child(2) {
    animation-delay:.1s;  
  }
  .back span:nth-child(3) {
    animation-delay:.2s;
  }
  .back span:nth-child(4) {
    animation-delay:.3s;  
  }
  .back span:nth-child(5) {
    animation-delay:.4s;
  }
  .back span:nth-child(6) {
    animation-delay:.5s;  
  }
  .back span:nth-child(7) {
    animation-delay:.6s;
  }
  .back span:nth-child(8) {
    animation-delay:.5s;
  }
  .back span:nth-child(9) {
    animation-delay:.8s;
  }
  .back span:nth-child(10) {
    animation-delay:.9s;
  }
  .back span:nth-child(11) {
    animation-delay:.10s;
  }
  .back span:nth-child(12) {
    animation-delay:.11s;
  }
 



</style>
