<template>
  <div class="pageCon">
    <!--<meta name="viewport" content="width=device-width, initial-scale=1.0">-->
    <div class="headSec">
      <div class="headWrapper">
        <div class="headGoldGrad">
          <!-- The container for the the welcome to/title/buttons on the landing page-->
          <div class="titleSecContainer">
            <p class="green-box-message">Welcome To</p>
            <h1>Treixatek</h1>
            <div></div>
            <div class="titlebox">

            </div>
            <div></div>
          </div>

        </div>
        <div class="headDivider"></div>
        <div class="headBlueGrad"></div>
      </div>
      


      <a href="#home">
        <img class="scrollArrow" src="/Websitemedia/Icons/arrow.png" alt="arrow">
      </a>
      <a id="home"></a>
    </div>
    
    <div class="containSec">
      <div class="line"></div>
      <div class="GridSec">
        <div class="containerH">
          <a href="/about">
            <img src="/Websitemedia/blueGrad.png" alt="Blue Gradient" class="imageH">
            <img src="/Websitemedia/Icons/Software.png" alt="Robot" class="hoverIcon">
            <div class="overlay">
              <div class="textBlue">Software</div>
            </div>
          </a>
        </div>

        <div class="containerHM">
          <a href="/games">
            <img src="/Websitemedia/goldGrad.png" alt="Gold Gradient" class="imageH">
            <img src="/Websitemedia/Icons/Games.png" alt="Character Shooting" class="hoverIcon">
            <div class="overlay">
              <div class="textGold">Games</div>
            </div>
          </a>
        </div>

        <div class="containerHL">
          <a href="/devlogs">
            <img src="/Websitemedia/greenGrad.png" alt="Green Gradient" class="imageH">
            <img src="/Websitemedia/Icons/Devlogs.png" alt="Character with Laptop" class="hoverIcon">
            <div class="overlay">
              <div class="textGreen">Devlogs</div>
            </div>
          </a>
        </div>
      </div>
    </div>
    
    <div class="containerSec">
      <div class="firstPan">
        <a href="/games">
          <img src="/Websitemedia/Icons/GamesWhite.png" alt="Character Shooting" class="panelImage1">
        </a>
        
        <div>
          <a href="/games">
            <h2 class="headingR">Our Games</h2>
          </a>
          <p class="headPara">Lorem ipsum dolor sit amet, consectetur adipiscing elit. Duis sit amet tempor nunc. Ut scelerisque luctus eleifend. Aenean ut finibus nisi.</p>
        </div>
      </div>
      <div class="lastPan">
        <a href="/software">
          <img src="/Websitemedia/Icons/SoftwareBlue.png" alt="Robot" class="panelImageLast">
        </a>

        <div>
          <a href="/software">
            <h2 class="headingLastR">Our Software</h2>
          </a>
          <p class="headParaLast">Consectetur adipiscing elit. Quisque dictum lectus at massa interdum, eget pharetra ex iaculis. Mauris sit amet rhoncus risus. Phasellus ut scelerisque est.</p>
        </div>
      </div>
    </div>
    
    <div class="containerSec">
      <div class="galPan">
        <div class="galContainer">
          <img src="/Websitemedia/Gallery/Bridge.png" alt="Standoff Animation" class="galIm">
          <div class="overlay">
            <div class="textBlue">Software</div>
          </div>
        </div>

        <div class="galContainer">
          <img src="/Websitemedia/Gallery/Standoff.gif" alt="Standoff Animation" class="galIm">
          <div class="overlay">
            <div class="textBlue">Software</div>
          </div>
        </div>

        <div class="galContainer">
          <img src="/Websitemedia/Gallery/Jam Game.png" alt="Standoff Animation" class="galIm">
          <div class="overlay">
            <div class="textBlue">Software</div>
          </div>
        </div>

        
      </div>
    </div>
    
  </div>
</template>

<script>
export default {
  
  components: {
    
  },
  head(){
    return {
      title: "Treixatek | Game Development",
      meta: [
        {
          hid: "description",
          name: "description",
          content: "Treixatek is an small indie development studio",
        }
      ]
    }
  }
}
</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Quicksand:wght@400;500;600;700&display=swap');
html {
  scroll-behavior: smooth;
}
.GridSec {
  position: absolute;
  top: 0;

  width: 100%;
  height: 50px;
  display: grid;
  grid-template-columns: repeat(auto-fill, minmax(260 px, 1fr));

}
.titleSecContainer{
  background: rgba(255, 255, 255, 0.2);
  width: 550px;
  height: 298px;
  margin-top: 20vh;
  margin-left: 103px;
  
  max-width: 25rem;
  text-align: left;
  display: inline-block;

}
.titlebox{
  background: tomato;
}
.headSec {
  width: 100%;
  position: relative;
  top: 100%;
  background: red;
}
.headWrapper {
  display: grid;
  grid-template-columns: 65.1% 0.9% 34%;
}
.headGoldGrad {
  height: 100vh;
  background: radial-gradient(70.74% 73.89% at 75.03% 85.5%, #FFD568 0%, #FFB74B 100%);

  display: grid;
  grid-template-rows: 33.3333333333% 33.3333333333% 33.3333333333%;
}
.headBlueGrad {
  height: 100vh;
  background: linear-gradient(159.9deg, #00C0FE 0%, #008FFC 97.54%);
}
.headDivider {
  height: 100vh;
  background: #fff;
}
.scrollArrow {
  width: 3%;
  position: absolute;
  bottom: 15%;
  left: 47%;
  
  animation: arrowAnim 1.5s ease-out infinite;
}
@keyframes arrowAnim {
  0% {
    bottom: 15%;
    opacity: 0;
  }

  40% {
    
    opacity: 1;
  }
  60% {
    
    opacity: 1;
  }

  100% {
    bottom: 4%;
    opacity: 0;
  }
}

.containSec {
  margin-top: 2%;
  margin-bottom: 2.8%;
  width: 100%;
  padding-top: 16.5%;

  position: relative;
  
}
.line {
  position: absolute;
  top: 50%;
  width: 100%;
  padding-top: 0.5%;

  background-color: rgba(255, 255, 255, 0.2);

  box-shadow: 0px 2px 5px rgba(0,0,0,0.1);
}


.container {
  margin: 0;
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
}

.image{
  width: 100%;
  
  border-bottom-color: #00C3FF;
  border-bottom-style: solid;
  border-bottom-width: 5px;

  box-shadow: 0px 3px 5px #121722;
}
.title {
  font-family: 'Quicksand', sans-serif;
  font-weight: 300;
  font-size: 100px;
  color: #35495e;
  letter-spacing: 1px;
}
.subtitle {
  font-weight: 300;
  font-size: 42px;
  color: #526488;
  word-spacing: 5px;
  padding-bottom: 15px;
}

/* HOVER BOXES */
.containerH {
  position: absolute;
  top: 0;
  left: 10%;
  width: 17%;
  
  transform: rotateZ(0deg);
  transition: 0.7s ease;
}
.containerHM {
  width: 17%;
  position: absolute;
  top: 0;
  left: 50%;
  transform: translate(-50%, 0%);

  transition: 0.7s ease;
}
.containerHL {
  position: absolute;
  top: 0;
  right: 10%;
  width: 17%;
  
  transform: rotateZ(0deg);
  transition: 0.7s ease;
}

.imageH {
  display: block;
  width: 100%;

  
  box-shadow: 0px 0px 10px  rgba(0,0,0,0.6);
  -moz-box-shadow: 0px 0px 10px  rgba(0,0,0,0.6);
  -webkit-box-shadow: 0px 0px 10px  rgba(0,0,0,0.6);
  -o-box-shadow: 0px 0px 10px  rgba(0,0,0,0.6);
  border-radius: 20px;
  /*
  box-shadow: 
    4px 4px 4px rgba(0,0,0,0.2),
    -4px -4px 4px rgba(191,191,191,0.1);
  
  border-width: 10px;
  border-radius: 20px;
  border-style: solid;
  border-color: #2c3040;

  transition: 0.3s ease;*/
}

.hoverIcon {
  width: 70%;
  height: auto;

  position: absolute;
  top: 15%;
  left: 15.5%;

  transition: 0.5s ease;
}


.overlay {
  position: absolute;
  bottom: 0;
  left: 0;
  right: 0;
  background-color: #2c3040;
  overflow: hidden;
  width: 100%;
  height: 0;
  border-radius:0px;
  border-bottom-right-radius: 10px;
  border-bottom-left-radius: 10px;
  transition: 0.3s ease;

  box-shadow: 0px -2px 3px rgba(0,0,0,0.3);
}

.containerH:hover {
  transform: rotateZ(-5deg)
  scale(1.1, 1.1);
}
.containerH:hover .overlay {
  height: 30%;
}
.containerH:hover .hoverIcon {
  top: 10%;
  left: 25%;
  width: 50%;
}
.containerHM:hover {
  position: absolute;
  left: 50%;

  transform: translate(-50%, 0%)
  scale(1.2, 1.2);
}
.containerHM:hover .overlay {
  height: 30%;
}
.containerHM:hover .hoverIcon {
  top: 10%;
  left: 25%;
  width: 50%;
}
.containerHL:hover {
  transform: rotateZ(5deg)
  scale(1.1, 1.1);
}
.containerHL:hover .overlay {
  height: 30%;
}
.containerHL:hover .hoverIcon {
  top: 10%;
  left: 25%;
  width: 50%;
}
/*  */
.textBlue {
  background: -webkit-linear-gradient(right, #0096fd, #00b7ff);
  background-clip: text;
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;

  white-space: nowrap; 
  font-size: 1.11vw;
  font-weight: bold;
  letter-spacing: 5px;
  position: absolute;
  overflow: hidden;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  -ms-transform: translate(-50%, -50%);
}
.textGold {
  background: -webkit-linear-gradient(right, #ffb346, #ffd346);
  background-clip: text;
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;

  white-space: nowrap; 
  font-size: 1.11vw;
  font-weight: bold;
  letter-spacing: 5px;
  position: absolute;
  overflow: hidden;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  -ms-transform: translate(-50%, -50%);
}
.textGreen {
  background: -webkit-linear-gradient(right, #1ad9cf, #2be8b0);
  background-clip: text;
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;

  white-space: nowrap; 
  font-size: 1.11vw;
  font-weight: bold;
  letter-spacing: 5px;
  position: absolute;
  overflow: hidden;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  -ms-transform: translate(-50%, -50%);
}

/* PANELS */
.firstPan {
  background-color: #008AFC;
  width: 100%;
  padding-top: 21%;
  display: block;

  position: relative;
  top: 100%;

  box-shadow: 0px -5px 5px rgba(0,0,0,0.3);
}
.panelImage1 {
  float: left;
  width: 12%;
  position: absolute;
  top: 20%;
  left: 20%;

  transition: 0.6s ease;
}
.panelImage1:hover {
  
  transform: scale(1.1, 1.1)
  rotate(-10deg)
  
}
.headingR {
  position: absolute;
  left: 35%;
  top: 30%;
  color: white;
  font-weight: 700;
  font-size: 1.6vw;

  transform: translateZ(0px);
  -webkit-transform: translateZ(0px);

  transition: 0.3s ease;
}
.headingR:hover {
  letter-spacing: 1px;
}
.headingR::before {
    content: '';
    position: absolute;
    bottom: 0;
    left: 0;
    width: 100%;
    height: 3px;
    background: white;

    transition: transform 0.3s;
    transform-origin: right;
    transform: scaleX(0);
}
.headingR:hover::before {
    transition: transform 0.3s;
    transform-origin: left;
    transform: scaleX(1);
}

.headPara {
  width: 30%;
  position: absolute;
  left: 35%;
  top: 45%;

  text-align: left;
  word-wrap: normal;
  color: white;
  font-weight: 500;
  font-size: 1.11vw;

  transform: translateZ(0px);
  -webkit-transform: translateZ(0px);
}

.lastPan {
  background-color: white;
  width: 100%;
  padding-top: 21%;
  display: block;

  position: relative;
  top: 100%;
  transform: translateY(-20%);

  clip-path: polygon(100% 0, 100% 100%, 0% 100%, 0 20%);
  box-shadow: 0px 5px 5px rgba(0,0,0,0.6);
}
.panelImageLast {
  float: right;
  width: 12%;
  position: absolute;
  top: 20%;
  right: 20%;

  transition: 0.6s ease;
}
.panelImageLast:hover {
  
  transform: scale(1.1, 1.1)
  rotate(10deg)
  
}
.headingLastR {
  position: absolute;
  right: 35%;
  top: 30%;
  color: #008AFC;
  font-weight: 700;
  font-size: 1.6vw;

  transform: translateZ(0px);
  -webkit-transform: translateZ(0px);

  transition: 0.3s ease;
}
.headingLastR:hover {
  letter-spacing: 1px;
}

.headingLastR::before {
    content: '';
    position: absolute;
    bottom: 0;
    left: 0;
    width: 100%;
    height: 3px;
    background: #008AFC;

    transition: transform 0.3s;
    transform-origin: right;
    transform: scaleX(0);
}
.headingLastR:hover::before {
    transition: transform 0.3s;
    transform-origin: left;
    transform: scaleX(1);
}

.headParaLast {
  width: 30%;
  position: absolute;
  right: 35%;
  top: 45%;

  text-align: right;
  word-wrap: normal;
  color: #008AFC;
  font-weight: 500;
  font-size: 1.11vw;

  transform: translateZ(0px);
  -webkit-transform: translateZ(0px);
}

.galPan::after {
  content: '';
  clear: both;
  display: table;
  
}

.galContainer {
  float: left;
  width: 30%;

  margin-right: 30px;
  margin-left: 30px;
}

.galIm {
  width: 100%;
  border: #2c3040;
  border-width: 10px;
  border-style: solid;

  border-radius: 20px;

  box-shadow: 
    4px 4px 4px rgba(0,0,0,0.2),
    -4px -4px 4px rgba(191,191,191,0.1);
}

/* PAGE ANIMATIONS */
.pageCon {
  width: 100%;
  animation-timing-function: ease-out;
  animation: transitionIn 0.5s;
}
@keyframes transitionIn {
  from{
    opacity: 0;
    
    transform: translateY(5vh);
  }

  to {
    opacity: 1;
    
    transform: translateY(0);
  }
}
</style>
