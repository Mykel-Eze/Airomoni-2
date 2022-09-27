<template>
  <div id="nav">
    <Navbar />
      <div id="main-contents-wrapper">
        <router-view />
      </div>
    <Footer />
  </div>
</template>

<script>
import Navbar from "@/components/Navbar.vue";
import Footer from "@/components/Footer.vue";

// import M from 'materialize-css'
import $ from "jquery";
export default {
  components: {
    Navbar, Footer
  },
  mounted() {
    $(window).scroll(function () {
      $('nav.trans-nav').toggleClass('scrolled-nav', $(this).scrollTop() > 50);
    });


    /**
     * Determine the mobile operating system.
     * This function returns one of 'iOS', 'Android', 'Windows Phone', or 'unknown'.
     *
     * @returns {String}
     */
    function getMobileOperatingSystem() {
      let userAgent = navigator.userAgent || navigator.vendor || window.opera;

      // Windows Phone must come first because its UA also contains "Android"
      if (/windows phone/i.test(userAgent)) {
        return "Windows Phone";
      }

      if (/android/i.test(userAgent)) {
          return "Android";
      }

      // iOS detection from: http://stackoverflow.com/a/9039885/177710
      if (/iPad|iPhone|iPod/.test(userAgent) && !window.MSStream) {
          return "iOS";
      }

      return "unknown";
    }

    if((getMobileOperatingSystem() == "unknown") || (getMobileOperatingSystem() == "Windows Phone")) {
      document.querySelectorAll('.unknown-device').forEach(item => {
        item.style.display = "block"
      })
    }
    else if(getMobileOperatingSystem() == "iOS") {
      document.querySelectorAll('.ios-device').forEach(item => {
        item.style.display = "block"
      })
    }
    else {
      document.querySelectorAll('.andriod-device').forEach(item => {
        item.style.display = "block"
      })
      console.log(getMobileOperatingSystem())
    } 
    
  }
}
</script>

<style src=".\assets\css\fonts.css"></style>
<style src=".\assets\css\styles.css"></style>

<style>
/* div#main-contents-wrapper {
  padding-top: 80px;
} */
</style>

