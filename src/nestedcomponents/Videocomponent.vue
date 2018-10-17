<template>
<div>
  <video-bg class="videobg" :sources="['static/surf.mp4']"> 
  <div class="header-overlay"></div>
  <div class="cta">If you want to add content here, a slot is waiting!</div>
</video-bg>



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

.videobg{
  text-align: center;
}

.cta{
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  border: solid 1px;
  padding: 20px;
  z-index: 2;
 
}


/* .cta:hover{ */
  /* background: red; */
  /* color: white; */
  /* } */

.cta:hover{
  border: solid white 1px;
  color: white;
  font-weight: 500;
}


.header-overlay{
  height:100vh;
  position: absolute;
  top:0;
  left:0;
  width:100%;
  z-index:1;
  /* background:#225470; */
  background:#000000;
  opacity:0.35;
  overflow:hidden;
}



@media(max-width:960px){
  .container{
    padding-right:3rem;
    padding-left:3rem;
  }
}

</style>
