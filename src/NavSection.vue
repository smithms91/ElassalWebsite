<template>
  <div id="nav-section-container">
    <div id="nav-section">
      <div class="logo-nav">
        <div class="left">
          <img src="./assets/logo.png" alt="">
          <div class="text">
            <h1>Elassal &amp; Associates</h1>
            <p>+1 (313) LAW - HELP</p>
          </div>
        </div>
        <div class="right">
          <div class="sandwich" @click="navOpen = !navOpen">
            <div class="line"></div>
            <div class="line"></div>
            <div class="line"></div>
          </div>
        </div>
      </div>

      <div class="content">
        <h1>Elassal &amp; Associates</h1>
        <button><i class="fas fa-phone"></i>+1 (313) LAW-HELP</button>
      </div>
    </div>

    <transition name="slide">
      <div class="modal" v-if="navOpen">
        <div class="close" @click="navOpen = !navOpen"><i class="fas fa-times"></i></div>
        <h3>Menu</h3>
        <ul>
          <li>Home</li>
          <li>About</li>
          <li @click="toggleDropdown = !toggleDropdown">
            Attorney Profiles 
            <i class="fas fa-arrow-down" v-if="!toggleDropdown"></i>
            <i class="fas fa-arrow-up" v-if="toggleDropdown"></i>
            </li>
            <ul class="inside" v-if="toggleDropdown">
              <li>Lawrence Elassal</li>
              <li>Nicholas Curtis</li>
            </ul>
          <li @click="toggleAreas = !toggleAreas">
            Areas of Practice 
            <i class="fas fa-arrow-down" v-if="!toggleAreas"></i>
            <i class="fas fa-arrow-up" v-if="toggleAreas"></i>
            </li>
            <ul class="inside" v-if="toggleAreas">
              <li>Criminal</li>
              <li>Drunk Driving</li>
              <li>Traffic Violations</li>
              <li>Gun &amp; Drug Crimes</li>
              <li>DUI / OWI / MIP</li>
              <li>Personal Injury</li>
              <li>Auto Accidents</li>
              <li>Slip and Fall</li>
              <li>Divorce</li>
              <li>Wills &amp; Estates</li>
            </ul>
          <li>Blog</li>
          <li>Contact</li>
        </ul>
      </div>
    </transition>
  </div>
</template>

<script>
export default {
  name: "NavSection",
  data() {
    return {
      navOpen: true,
      toggleDropdown: false,
      toggleAreas: false
    }
  }
}
</script>

<style scoped>
  #nav-section {
    background-image: url('./assets/navbg.png');
    background-size: cover;
    /* background-position:  */
    height: 600px;
    padding: 40px 20px;
    clip-path: polygon(0 0, 100% 0, 100% 90%, 0 100%);
    z-index: 102;
  }

  .logo-nav {
    display: flex;
    align-items: center;
    justify-content: space-between;
    width: 100%;
  }

  .left {
    display: flex;
    align-items: center;
    color: #eee;
  }

  .left img {
    width: 40px;
  }
  
  .text {
    margin-left: 10px;
  }

  .text h1 {
    font-size: 16px;
    font-family: 'Lora', serif;
  }

  .text p {
    color: #A2B9D1;
    font-size: 12px;
    margin: -3px 0;
    letter-spacing: 1px;
    text-align: center;
    font-family: 'Open Sans', sans-serif;
  }

  .sandwich {
    width: 40px;
  }

  .line {
    height: 2px;
    margin: 6px;
    background-color: #eee;
  }


  .content {
    display: flex;
    flex-direction: column;
    align-items: center;
    margin-top: 125px;
    color: #eee;
    font-family: 'Merriweather', sans-serif;
  }

  .content h1 {
    font-size: 40px;
    text-align: center;
    margin-bottom: 40px;
  }

  .content button {
    padding: 15px;
    background: #053D61;
    color: white;
    border: none;
    border-radius: 5px;
    font-family: 'Open Sans', sans-serif;
    font-size: 16px;
  }

  .content button i {
    margin-right: 10px;
  }




  /* Modal */

  .modal {
    height: 100vh;
    width: 250px;
    background-color: rgba(50,50,50,.95);
    position: fixed;
    top: 0;
    bottom: 0;
    right: 0;
    text-align: left;
    color: #eee;
    padding: 20px;
    overflow-y: scroll;
    z-index: 200;
  }

  .modal .close {
    position: absolute;
    top: 10px;
    right: 20px;
    font-size: 30px;
  }

  .modal h3 {
    font-size: 36px;
    margin: 15px 0 10px 0;
    font-family: 'Open Sans', sans-serif;
    border-bottom: 1px solid grey;
    padding-bottom: 10px;
  }

  .modal ul {
    list-style-type: none;
    font-size: 20px;
    font-family: 'Open Sans', sans-serif;
  }

  .modal ul li {
    margin-bottom: 20px;
    font-family: 'Open Sans', sans-serif;
    
  }

  .inside li {
    margin-left: 20px;
    font-size: 14px;
  }

  li i {
    margin-left: 10px;
    font-size: 16px;
  }

  .slide-enter-active, .slide-leave-active {
    transition: all .5s;
  }

  .slide-enter, .slide-leave-to /* .fade-leave-active below version 2.1.8 */ {
    transform: translateX(100%);
    opacity: 0;
  }
</style>


