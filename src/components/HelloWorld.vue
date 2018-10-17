<template>
  <div>

    <nav >
    <div class="nav-wrapper">
     <a href="#" class="brand-logo">Web Zone</a>
     <ul class="right hide-on-med-and-down">
       <li><a href="#" class="red">Home</a></li>
       <li><a href="#">Blog</a></li>
       <li><a href="#">Theme</a></li>
       <li><a href="#">About</a></li>
       <li><a href="#">Contact</a></li>
     </ul>
    </div>
    </nav>



    
   
    
    <!-- 123 -->
  <Videocomponent/>

    <section class="section section-a">
    <div class="container">
      <h2>Section A</h2>
      <p>Lorem ipsum dolor, sit amet consectetur adipisicing elit. Unde, impedit amet minima iste autem cumque et maiores blanditiis doloribus aut dolorum quaerat non est voluptatum, tempore ut dolorem voluptas quod quae accusantium, ex inventore ducimus. Beatae mollitia exercitationem, quam similique, consectetur ratione reprehenderit delectus neque eligendi facere soluta dolor ducimus!</p>
    </div>
  </section>
  <section class="section section-b">
    <div class="container">
      <h2>Section B</h2>
      <p>Lorem ipsum dolor, sit amet consectetur adipisicing elit. Unde, impedit amet minima iste autem cumque et maiores blanditiis doloribus aut dolorum quaerat non est voluptatum, tempore ut dolorem voluptas quod quae accusantium, ex inventore ducimus. Beatae mollitia exercitationem, quam similique, consectetur ratione reprehenderit delectus neque eligendi facere soluta dolor ducimus!</p>
    </div>
  </section>
  
  
  </div>



</template>

<script>

import Videocomponent from './../nestedcomponents/Videocomponent'

export default {
  name: 'HelloWorld',
  components: {
    Videocomponent,
  },
  ready() {

         console.log("hi?")
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

    
    nav{
      position: fixed;
      background: rgba(0, 0, 0, 0.2);
      padding:0px 20px;
      z-index: 100;
    }


    nav li a:hover{
      background: red;
    }



.section{
  padding:20px 0;
  width: 100%;
  /* border: solid 1px; */
  margin:0;
}

.section-b{
  background-color:#333;
  color:#fff;
  margin:0;
  
  /* border: solid red 2px; */
}
</style>
