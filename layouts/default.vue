<template>
  <div class="container">
      <AppHeader/>
      <SocialBar/>
      <nuxt />
  </div>
</template>

<script>
import AppHeader from "../components/AppHeader";
import SocialBar from "../components/SocialBar";
export default {
    components: {
        AppHeader,
        SocialBar
    }
};
</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Poppins:wght@400;600&family=Rakkas&display=swap');

html {
    -webkit-text-size-adjust: none;
    -webkit-font-smoothing: subpixel-antialiased;
    -webkit-font-smoothing: antialiased;
  }
  
  a,body,button,div,footer,form,h1,h2,h3,h4,header,html,img,input,label,li,nav,p,select,span,table,textarea,ul {
    margin: 0;
    padding: 0;
    border: 0;
    font: inherit;
    font-family: inherit;
    font-size: 100%;
  }
  
  li,ul {
    list-style: none;
  }
  
  button,input,select,textarea {
    display: block;
    box-sizing: border-box;
    border-radius: 0;
    outline: none;
    border: none;
    background: none;
    color: inherit;
  }
  
  button:focus,input:focus,textarea:focus {
    outline: none;
  }
  
  button:hover,input[type=submit]:hover {
    cursor: pointer;
  }
  
  input::-ms-clear {
    display: none;
  }
  
  textarea {
    overflow: auto;
  }
  
  a {
    color: inherit;
    text-decoration: none;
    transition: ease-in 400ms;
  }
  
  a,img,picture,svg,video {
    display: block;
  }
  
  img,video {
    width: 100%;
    height: auto;
  }
  
  iframe,svg {
    width: 100%;
    height: 100%;
  }
  
  iframe {
    position: absolute;
    top: 0;
    left: 0;
  
  }
  

body{
    background-color: #1A1A1A;
    color:#F5F5F5;
    font-family: 'Poppins', sans-serif;
    padding: 40px 80px;
    margin: 0;
    line-height: 1.8em;
}
h1,h2,h3{
    font-family: 'Rakkas', cursive;
}
h1{
    font-size: 9em;
    line-height: 0.8em;
}
h2{
    font-size: 4em;
    line-height: 0.9em;
}
h3{
  font-size: 2em;
    line-height: 0.9em;
}
/*outline strokes*/
@supports (-webkit-text-stroke: 1.5px #f5f5f5) {
    .outlines {
    -webkit-text-stroke: 1.5px #f5f5f5;
    -webkit-text-fill-color: #1A1A1A;
  }
}
.red-title{
    color: #800000;
}
.text-align-center{
  text-align: center;
  margin-top: -40px;
}
a:hover{
  transition: ease-in 400ms;
  color: #800000;
}
</style>