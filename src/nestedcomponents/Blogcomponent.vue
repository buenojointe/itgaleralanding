<template>
    <div class="section">
        <div class="container">
          <h2>Section Blog</h2>
          <h1 class="title is-1">Your Window</h1>
          <h2 class="title is-2">
              Width: {{ window.width }},
              Height: {{ window.height }}
          </h2>

        </div>
        
        

  </div>
</template>

<script>



export default {
  name: 'Blog',
  data () {
    return {
      msg: 'Welcome to Your Vue.js App',
      window: {
      width: 0,
      height: 0
    }
    }
  },
  
}
</script>


<style scoped>


.cta{
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
    color:white;

}





.section{
  width: 100%;
  height: 100vh;
  background-color: #D3D3D3;
}



</style>
