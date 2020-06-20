<template>
  <div class="text-align-center">
    <section class="hero full-height">
      <span>MY FRIENDS CALL ME,</span>
      <h1 class="outlines">MEKEL,<br>VERELLINO</h1>
      <span>I DO WEB DESIGN & DEVELOPMENT.<br>
            CALL ME A VISUAL DEVELOPER. SOUNDS LEGIT, RIGHT?</span>
    </section>
    <section class="showcase full-height">
      <h2 class="red-title left-align">RECENT WORKS</h2>
      <flickity  class="flickity" ref="flickity" :options="flickityOptions">
        <div class="carousel-cell">
          <a href="http://disco-tique.com"></a>
          <h2>DISCOTIQUE</h2>
        </div>
      </flickity>
    </section>
    <section class="aboutme">
      <div class="pma">
        <img src="https://media.giphy.com/media/6bSoMak3jOH4s/giphy.gif" class="giphy-embed" alt="punk">
        <h2 class="red-title">FOR THE LOVE OF PUNK ROCK</h2>
        <h2 class="red-title">AND CHEAP BOOZE,</h2>
        <h2 class="red-title">KEEP THE PMA!</h2>
      </div>
      <div class="bio full-height">
        <!--<h1 class="outlines right-align">MICHAEL<br>VERELLINO</h1>-->
        <div class="bio-right">
          <img class="ava" src="../assets/Mekel-Face-Black-White.jpg" alt="Mekel's Face">
          <span>v1.0 || 2020</span>
        </div>
        <div class="bio-left">
          <h2 class="red-title">A BRIEF INQUIRY</h2>
          <br>
          <p>IT'S PRONOUNCED /mɛk hɛl/. IT'S JAVANESE PRONUNCIATION DUDE.
          <br>BASED IN YOGYAKARTA, INDONESIA.</p>
          <br><br>
          <p>🤙 SUP!
            <br><br>
            I'VE BEEN WORKING TOGETHER WITH CREATIVE MINDS ACROSS THIS PLANET CALLED EARTH. EXPLORING VISUALS IN THE WORLD WIDE WEB AND CREATING PERSONAS FOR THE TEAM OR INDIVIDUALS I'VE BEEN WORKING WITH. I HAVE BEEN FREELANCING SINCE 2014,
            ALWAYS AVAILABLE FOR CREATING NEW EXPERIENCES AND BUILDING VIRTUAL WORLDS.
            <br><br> GET IN TOUCH, LET'S GET SUM BEER.</p>
          <br>
          <h3><a href="mailto:verellino@gmail.com?subject=WASSUP MEKEL!🤙"><fa :icon="faEnvelope" /> | | EMAIL ME!</a></h3>
        </div>
      </div>
    </section>
    <section class="contactme full-height">
      <h1 class="outlines">LET'S WORK TOGETHER</h1>
      <a href="/">@verellino</a>
      <div class="footer">
        <div class="footer-logo">
          <img src="../assets/shaka.svg" alt="shaka hand sign">
        </div>
        <span>© 2020 | ALL RIGHTS RESERVED.</span>
        <span>MICHAEL VERELLINO</span>
      </div>
    </section>
  </div>
</template>

<script>
import { faEnvelope } from '@fortawesome/fontawesome-free-solid'
export default {
  head() {
    return {
      title: 'Mekel Verellino - Web Design & Development',
      meta: [
        {
          hid: "description",
          name: "description",
          content: "Mekel Verellino is a Freelance Web Designer and Developer from Yogyakarta, Indonesia."
        }
      ]
    };
  },
  data () {
    return {
      flickityOptions: {
        initialIndex: 0,
        prevNextButtons: true,
        draggable: true,
        wrapAround: true,
        fade: true,
      }
    }
  },
  
    computed: {
      faEnvelope () {
         return faEnvelope
      }
    },
};

</script>

<style>
.full-height{
  height: 100vh;
  display: flex;
  flex-direction:column;
  align-items: center;
  justify-content: center;
}
.flickity{
  margin-top: 50px;
  width: 95vw;
  height: 80vh;
}
.carousel{
  position: relative;
  width: 100%;
  height: 100%;
}
.carousel-cell {
  width: 70%;
  height: 100%;
  margin-right: 50px;
  background: linear-gradient(180deg, rgba(128, 0, 0, 0.8) 0%, rgba(0, 0, 0, 0.5) 100%), url(../assets/Discotique-Fashion-Ecommerce.jpg);
  background-size: cover;
  transition: background ease-in 400ms;
}
.carousel-cell a {
  width: 100%;
  height: 100%;
}
.carousel-cell h2{
  position: absolute;
  bottom: 10px;
  right: 5px;
}
.carousel-cell:active {
  background: url(../assets/Discotique-Fashion-Ecommerce.jpg);
  background-size: cover;
  transition: background ease-in 400ms;
}
.flickity-page-dots{
  bottom: -50px;
}
.dot.is-selected{
  transition: ease-in 300ms;
  background: #800000;
}
.pma{
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  height: 80vh;
}
.giphy-embed{
  width: 250px;
  margin-bottom: 20px;
}
.bio{
  display: flex;
  flex-direction: row-reverse;
  align-items: flex-start;
}
.bio-left{
  width: 50%;
  height: 100%;
  text-align: left;
  padding-right: 20px;
}
.bio-right{
  width: 50%;
  display: flex;
  flex-direction:column;
  align-items:flex-end;
  position: sticky;
  position: -webkit-sticky;
  top: 50px;
}
.ava{
  width: 500px;
  background: #000;
}
.contactme{
  position: relative;
}
.footer{
  position: absolute;
  bottom: 0;
  display: flex;
  flex-direction:column;
  align-items: center;
  justify-content: center;
}
.footer-logo{
  width: 40px;
}
</style>