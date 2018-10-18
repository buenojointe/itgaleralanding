<template>
  <div>

    <nav >
    <div class="nav-wrapper">
     <a href="#" class="brand-logo">itgalera.io</a>
     <!-- <a href="#" data-target="mobile-demo" class="sidenav-trigger"><i class="material-icons"></i></a> -->
     <ul class="right hide-on-med-and-down">
       <li><a href="#" class="red">Home</a></li>
       <li><a href="#">Blog</a></li>
       <li><a href="#">Portfolio</a></li>
       <li><a href="#">About</a></li>
       <li><a href="#">Contact</a></li>
     </ul>
    </div>
    </nav>



    
   
    
    <!-- 123 -->
  <YoutubeFullpagecomponent/>
  <!-- <Videocomponent/> -->
  
  <Blogcomponent/>
  <Portfoliocomponent/>
  
  <Aboutcomponent/>
  <Contactscomponent/>
  



  
  
  </div>



</template>

<script>

import Videocomponent from './../nestedcomponents/Videocomponent'
import Portfoliocomponent from './../nestedcomponents/Portfoliocomponent'
import Blogcomponent from './../nestedcomponents/Blogcomponent'
import Aboutcomponent from './../nestedcomponents/Aboutcomponent'
import Contactscomponent from './../nestedcomponents/Contactscomponent'
import YoutubeFullpagecomponent from './../nestedcomponents/YoutubeFullpagecomponent'

export default {
  name: 'HelloWorld',
  components: {
    Videocomponent,Blogcomponent,Portfoliocomponent,Aboutcomponent,Contactscomponent,YoutubeFullpagecomponent
  },
  data () {
    return {
      msg: 'Welcome to Your Vue.js App'
    }
  },
  

}

     
 


</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

.brand-logo{
  font-family: Work Sans;
  font-size:250%;
  font-weight: 400;

}

    
nav{
  position: fixed;
  background: rgba(0, 0, 0, 0.2);
  padding:0px 20px;
  z-index: 100;
}


nav li a:hover{
  background: red;
  color: white;
  }






</style>
