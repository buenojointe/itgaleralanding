<template>
<div>
  
  <header class="v-header container">
    <div class="fullscreen-video-wrap">
      <video muted src="static/surf.mp4" autoplay="true" loop="true" type="video/mp4"></video>
    </div>
    <div class="header-overlay"></div>
    <div class="header-content text-md-center">
      <h1>Need a Landing Page?</h1>
      <p>Contact me!</p>
      <a href="https://web.telegram.org/#/im?p=@RFahreev" class="btn"><img src="static/tglink.png" alt=""></a>
    </div>
  </header>



</div>

</template>


<script>

import VueVideoBackground from 'vue-video-background'

export default {
  name: 'Videocomponent',
  data () {
    return {
      msg: 'Welcome to Your Vue.js App'
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>


.v-header{
  height:100vh;
  display:flex;
  align-items:center;
  color:#fff;
  /* z-index: 5; */
}

.container{
  max-width:960px;
  padding-left:1rem;
  padding-right:1rem;
  margin:auto;
  text-align:center;
  /* z-index: 6; */
}

.fullscreen-video-wrap{
  position:absolute;
  top:0;
  left:0;
  width:100%;
  height:100vh;
  overflow:hidden;
  margin-left:auto;
  margin-right:auto;
  z-index:-100;
  text-align:center;
}

.fullscreen-video-wrap video{
  min-height:100vh;
  min-width:100%;
  overflow:hidden;
}

.header-overlay{
  height:100vh;
  position: absolute;
  top:0;
  left:0;
  width:100%;
  z-index:1;
  background:#225470;
  opacity:0.65;
  overflow:hidden;
}

.header-content{
  margin-left:auto;
  margin-right:auto;
  z-index:2;

}

.header-content h1{
  font-size:50px;
  margin-bottom:10px;
}

.header-content p{
  font-size:1.5rem;
  display:block;
  padding-bottom:2rem;
}


.btn{
  background: #34b3a0;
  color:#fff;
  font-size:1.2rem;
  /* padding:auto; */
  height: 100px;
  width: 200px;
  /* padding: 1rem 2rem; */
  text-decoration: none;
}

.btn:hover{
  background: #05B200;

}

@media(max-width:960px){
  .container{
    padding-right:3rem;
    padding-left:3rem;
  }
}

</style>
