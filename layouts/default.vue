<template>
  <div>
    <AppHeader/>
    <nuxt />
    <Footer/>
  </div>
</template>

<script>
import AppHeader from '../components/AppHeader';
import Footer from '../components/Footer';

export default {
  components:{
    AppHeader,
    Footer
  }
}
</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Nunito:ital,wght@0,300;0,400;0,600;0,700;0,800;0,900;1,300;1,400;1,600;1,700;1,800;1,900&display=swap');
*{
  box-sizing: border-box;
  margin: 0;
  padding: 0;
}

html{
  font-size: 16px;
  word-spacing: 1px;
  -ms-text-size-adjust: 100%;
  -webkit-text-size-adjust: 100%;
  box-sizing: border-box;

  padding: 0;
}

body{
  /*font-family: 'Tajawal', sans-serif;*/
  font-family: 'Nunito', sans-serif;
  font-size: 1rem;
  line-height: 1.6;
  background-color: #F2F4F8;
  /*background-color: #394051;*/
  /*background-image: url('../static/Websitemedia/StripBGDark.png');*/
}

a{
  color: #666;
  text-decoration: none;
}
ul{
  list-style: none;
  
}

.container{
  margin: 2rem auto;
  overflow: hidden;
  padding: 1rem 2rem;
  background: #2f2f2f;
}
</style>
