<template>
  <div class="text-align-center">
    <section class="hero full-height">
      <h1 class="outlines">MEKEL
        <br>VERELLINO
      </h1>
      <span>I DO WEB DESIGN & FRONT-END DEVELOPMENT.
        <br>CALL ME A VISUAL DEVELOPER. SOUNDS LEGIT, RIGHT?
      </span>
    </section>
    <section class="showcase left-align">
      <h2>RECENT WORKS</h2>
      <div class="project-container">
        <div class="project left-align">
          <img class="project-img">
          <h4>PROJECT NAME</h4>
          <span>E COMMERCE / DIRECTION / UX</span>
        </div>
        <div class="project left-align">
          <img class="project-img">
          <h4>PROJECT NAME</h4>
          <span>E COMMERCE / DIRECTION / UX</span>
        </div>
        <div class="project left-align">
          <img class="project-img">
          <h4>PROJECT NAME</h4>
          <span>E COMMERCE / DIRECTION / UX</span>
        </div>
      </div>
    </section>
    <section class="aboutme">
      <div class="bio full-height">
        <!--<h1 class="outlines right-align">MICHAEL<br>VERELLINO</h1>-->
        <div class="bio-right">
          <img class="ava" src="../assets/Mekel-Face-Black-White.jpg" alt="Mekel's Face">
          <span>v1.0 || 2020</span>
        </div>
        <div class="bio-left">
          <h2 class="red-title">A BRIEF INQUIRY</h2>
          <p class="hyphenate">IT'S PRONOUNCED /mɛk hɛl/.
            <br>IT'S JAVANESE PRONUNCIATION, BUT IT IS SPELLED MICHAEL ON MY BIRTH CERTIFICATE 😜
          </p>
          <br>
          <p class="hyphenate">
            🤙 SUP!
            <br>
            <br>I'M A HUMAN BEING WHO IS ALSO A FREELANCER BASED IN YOGYAKARTA, INDONESIA.
            <br>
            <br>I'VE BEEN WORKING TOGETHER WITH CREATIVE MINDS ACROSS THIS PLANET CALLED EARTH.
            <br>
            <br>EXPLORING VISUALS IN THE WORLD WIDE WEB AND CREATING PERSONAS FOR THE TEAM OR INDIVIDUALS. I HAVE BEEN FREELANCING SINCE 2014,
            ALWAYS AVAILABLE FOR CREATING NEW EXPERIENCES AND BUILDING VIRTUAL WORLDS.
            <br>
            <br>GET IN TOUCH, LET'S GET SUM BEER.
          </p>
          <br>
          <a href="mailto:verellino@gmail.com?subject=WASSUP MEKEL!🤙">LET'S JOIN FORCES!</a>
        </div>
      </div>
    </section>
    <section class="contactme full-height">
      <h1 class="outlines">LET'S WORK TOGETHER</h1>
      <a href="/">@verellino</a>
      <div class="footer">
        <span>©2020 | ALL RIGHTS RESERVED.</span>
      </div>
    </section>
  </div>
</template>

<script>
export default {
  head() {
    return {
      title: "Mekel Verellino - Web Design & Development",
      meta: [
        {
          hid: "description",
          name: "description",
          content:
            "Mekel Verellino is a Freelance Web Designer and Web Developer based in Yogyakarta, Indonesia. Focusing on UI UX Design, Front-end Development and Creative Direction."
        }
      ]
    };
  }
};
</script>

<style>
.full-height {
  min-height: 100vh;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
}
.left-align {
  align-items: start;
  text-align: left;
}
.showcase {
  min-height: 100vh;
  margin-bottom: 100px;
}
.project-container {
  margin-top: 40px;
  -ms-box-orient: horizontal;
  display: -webkit-box;
  display: -moz-box;
  display: -ms-flexbox;
  display: -moz-flex;
  display: -webkit-flex;
  display: flex;
  flex-wrap: wrap;
  align-items: start;
  justify-content: space-between;
}
.project {
  width: 48%;
  display: block;
  margin-bottom: 120px;
}
.project-img {
  width: 100%;
  height: 300px;
  background: no-repeat cover center;
  margin-bottom: 24px;
}
.pma {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  height: 80vh;
}
.giphy-embed {
  width: 250px;
  margin-bottom: 20px;
}
.bio {
  display: flex;
  flex-direction: row-reverse;
  align-items: flex-start;
}
.bio-left {
  width: 60%;
  height: 100%;
  text-align: left;
}
.bio-right {
  width: 40%;
  display: flex;
  flex-direction: column;
  align-items: flex-end;
  position: sticky;
  position: -webkit-sticky;
  top: 80px;
}
.ava {
  width: 75%;
  background: #000;
}
.contactme {
  position: relative;
}
.footer {
  position: absolute;
  bottom: 0;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
}
@media only screen and (min-device-width: 320px) and (max-device-width: 767px) and (-webkit-min-device-pixel-ratio: 2) {
  .project {
    width: 100%;
  }
  .showcase {
    height: auto;
  }
  .bio {
    flex-direction: column-reverse;
    justify-content: center;
  }
  .bio-right {
    width: 100%;
    align-items: center;
  }
  .bio-left {
    width: 100%;
    margin-bottom: 24px;
    padding: 0;
  }
}
</style>