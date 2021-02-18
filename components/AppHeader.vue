<template>
  <header class="header">
      <div class="logoIm" style="color: #31E89F">
          <img class="headIcon" src="./HeaderIms/Tlogo.webp" alt="Treixatek logo">
          <nuxt-link to="/" class="logo">T r e i x a <span style="color: #31E89F"> t</span><span style="color: #00C3FF"> e</span><span style="color: #008AFC"> k</span></nuxt-link>
      </div>

      <nav>
          <ul>
              <li><nuxt-link to="/games">
                <p class="gradTextGold">Games</p>
              </nuxt-link></li>
              <li><nuxt-link to="/devlogs">
                <p class="gradTextGreen">Devlogs</p>
              </nuxt-link></li>
              <li><nuxt-link to="/forum">
                <p class="gradTextRed">Forum</p>
              </nuxt-link></li>
              <li><nuxt-link to="/about">
                <p class="gradTextDefault">Login</p>
              </nuxt-link></li>
          </ul>
      </nav>
  </header>
</template>

<script>
export default {
    name: 'AppHeader'
}
</script>

<style>
    
    header {
        background: rgba(34, 37, 66, 0.21);
        display: grid;
        grid-template-columns: repeat(2,auto);

        position: fixed;
        top: 0;
        left: 0;

        width: 100%;
        z-index: 200;
    }
    .logoIm, li a {
        padding-top: 10px;
        padding-left: 15px;
        padding-bottom: 15px;
        
        display: block;
        
        background: white;
        width: 300px;
        /* blue: #00C3FF*/
    }
    .image {
        background: white;
    }
    .logo {
        position: relative;
        bottom: 0px;
        text-transform: uppercase;
        text-decoration: none;
        font-weight: bold;
        color: #a3bfe3;
        font-size: 21px;

        transition: 0.3s ease;
    }
    .logo:hover {
        letter-spacing: 0.5px;
    }
    .logo::before {
        content: '';
        position: absolute;
        bottom: 0;
        left: 0;
        width: 100%;
        height: 8%;
        background: #00b7ff;

        transition: transform 0.3s;
        transform-origin: right;
        transform: scaleX(0);
    }
    .logo:hover::before {
        transition: transform 0.3s;
        transform-origin: left;
        transform: scaleX(1);
    }
    .headIcon {
        position: relative;
        top: 7px;
        width: 35px;
        height: 35px;
    }
    nav {
        justify-self: right;
        width: 600px;
    }
    ul {
        list-style-type: none;
    }
    li {
        display: inline;
    }
    li a {
        border-top-style: none;
        border-bottom-style: solid;
        border-bottom-width: 5px;

        position: relative;
        bottom: 0px;
        border-right-style: none;
        border-bottom-color: #d4d7e3;
        border-bottom-style: solid;
        border-bottom-width: 0px;

        letter-spacing: normal;
        transition: 0.2s ease;

        color: #00b7ff;
        font-weight: 600;
        width: 125px;
        margin: 10px;
        font-size: .9em;
        text-align: center;
        padding: 0.9em 2em;
        display: inline-block;
        background-color: white;
    }
    li a:hover {
        border-bottom-width: 5px;
        bottom: 5px;
        /*background-color: #394051;
        border-bottom-color: #0c1125;*/

        letter-spacing: 2px;
    }
    li a:hover .gradTextGreen {
        background: -webkit-linear-gradient(right, #1ad9cf, #2be8b0);
        background-clip: text;
        -webkit-background-clip: text;
        -webkit-text-fill-color: transparent;
    }
    li a .gradTextGreen::before {
        content: '';
        position: absolute;
        bottom: 25%;
        left: 23%;
        width: 55%;
        height: 4%;
        background: -webkit-linear-gradient(right, #1ad9cf, #2be8b0);

        transition: transform 0.3s;
        transform-origin: right;
        transform: scaleX(0);
        
    }
    li a:hover .gradTextGreen::before {
        transition: transform 0.3s;
        transform-origin: left;
        transform: scaleX(1);
    }
    li a:hover .gradTextGold {
        background: -webkit-linear-gradient(right, #ffb346, #ffd346);
        background-clip: text;
        -webkit-background-clip: text;
        -webkit-text-fill-color: transparent;

    }
    li a:hover .gradTextGold {
        background: -webkit-linear-gradient(right, #ffb346, #ffd346);
        background-clip: text;
        -webkit-background-clip: text;
        -webkit-text-fill-color: transparent;
    }
    li a .gradTextGold::before {
        content: '';
        position: absolute;
        bottom: 25%;
        left: 28%;
        width: 45%;
        height: 4%;
        background: -webkit-linear-gradient(right, #ffb346, #ffd346);

        transition: transform 0.3s;
        transform-origin: right;
        transform: scaleX(0);
        
    }
    li a:hover .gradTextGold::before {
        transition: transform 0.3s;
        transform-origin: left;
        transform: scaleX(1);
    }
    li a:hover .gradTextRed {
        background: -webkit-linear-gradient(right, #FF2A90, #FF4063);
        background-clip: text;
        -webkit-background-clip: text;
        -webkit-text-fill-color: transparent;
    }
    li a .gradTextRed::before {
        content: '';
        position: absolute;
        bottom: 25%;
        left: 28%;
        width: 45%;
        height: 4%;
        background: -webkit-linear-gradient(right, #FF2A90, #FF4063);

        transition: transform 0.3s;
        transform-origin: right;
        transform: scaleX(0);
        
    }
    li a:hover .gradTextRed::before {
        transition: transform 0.3s;
        transform-origin: left;
        transform: scaleX(1);
    }
    li a .gradTextDefault::before {
        content: '';
        position: absolute;
        bottom: 25%;
        left: 30%;
        width: 41%;
        height: 4%;
        background: #00b7ff;

        transition: transform 0.3s;
        transform-origin: right;
        transform: scaleX(0);
        
    }
    li a:hover .gradTextDefault::before {
        transition: transform 0.3s;
        transform-origin: left;
        transform: scaleX(1);
    }
</style>