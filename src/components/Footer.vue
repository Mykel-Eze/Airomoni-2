<template>
    <footer id="footer" class="scrollspy">
        <div class="row">
            <div class="container">
                <div class="col s12 m4 text-center-xs*">
                    <div class="footer-logo">
                        <router-link to="/" tag="a" @click="scrollToTop()">
                            <img src="../assets/images/logo-2.svg" alt="Airomoni">
                        </router-link>
                    </div>
                    <div class="footer-about">
                        <p class="footer-about-txt">
                            AiroMoni is a product of Airopay Limited is a company registered in 
                            Nigeria (RC. 1203139). All rights reserved. Airopay is licensed by the 
                            Central Bank of Nigeria. “Airopay” and “Bankless World” are trademarks 
                            of Airopay Ltd Lekki, Lagos. Nigeria
                        </p>
                    </div>
                </div>
                <div class="col s12 m8 l7 pad0-xs offset-l1 f-links-wrapper">
                    <div class="col s6 m4 ddf">
                        <h5 class="footer-title">Quick Links</h5>
                        <ul class="footer-links-li">
                            <li>
                                <a href="/#sect-1" class="">About</a>
                            </li>
                            <li>
                                <router-link to="/faq" tag="a" @click="scrollToTop()" class="">FAQ</router-link>
                            </li>
                            <li class="unknown-device rel">
                                <router-link to="#" class="unknown-device-btn">Download App</router-link>
                                <div class="flex-div abs-btn-wrapper">
                                    <button class="btn app-store google-store" style="margin-right: 10px" onclick="window.location.href='https://play.google.com/store/apps/details?id=com.airopay.agents&hl=en&gl=US'">
                                        <img src="../assets/images/google-btn.svg" alt="play store">
                                    </button>
                                    <button class="btn app-store apple-store" onclick="window.location.href='https://apps.apple.com/tt/app/airomoni/id1560560802'">
                                        <img src="../assets/images/apple-btn.svg" alt="apple store">
                                    </button>
                                </div>
                            </li>
                            <li class="andriod-device">
                                <a href="https://play.google.com/store/apps/details?id=com.airopay.agents&hl=en&gl=US" target="_blank" class="">Get it on Play Store</a>
                            </li>
                            <li class="ios-device">
                                <a href="https://apps.apple.com/tt/app/airomoni/id1560560802" target="_blank" class="">Get it on App Store</a>
                            </li>
                        </ul>
                    </div>
                    <div class="col s6 m4 ddf">
                        <h5 class="footer-title">Legal</h5>
                        <ul class="footer-links-li">
                            <li>
                                <router-link to="/terms" tag="a" @click="scrollToTop()">Terms of Service</router-link>
                            </li>
                            <li>
                                <router-link to="/privacy-policy" tag="a" @click="scrollToTop()">Privacy Policy</router-link>
                            </li>
                            <!-- <li>
                                <router-link to="#">Disclaimers</router-link>
                            </li> -->
                        </ul>
                    </div>
                    <div class="col s12 m4 ddf">
                        <h5 class="footer-title">Contact</h5>
                        <ul class="footer-links-li">
                            <li>
                                <a href="mailto:agents@airomoni.com">agents@airomoni.com</a>
                            </li>
                            <li>
                                <a href="tel:+23401515591">+234 (01) 515 591</a>
                            </li>
                            <li>
                                <a href="tel:+2349133113205">+234 (0) 913 311 3205</a>
                            </li>
                            <li>
                                <a href="tel:+2349041111199">+234 (0) 904 111 1199</a>
                            </li>
                        </ul>
                    </div>
                </div>
                <div class="col s12 location-social-wrapper">
                    <div class="col s12 m5 l4 location-social">
                        <div class="location-div">
                            <div class="location-label">
                                <img src="../assets/images/nigeria.svg" alt="country-flag" id="country-flag">
                                <span id="country-name">Nigeria</span>
                            </div>
                        </div>
                        <div class="social-div">
                            <a href="https://www.facebook.com/Airomoni" target="_blank" class="social-link">
                                <img src="../assets/images/facebook.svg" alt="facebook">
                            </a>
                            <!-- <a href="https://twitter.com/" target="_blank" class="social-link">
                                <img src="../assets/images/twitter.svg" alt="facebook">
                            </a> -->
                            <!-- <a href="https://linkedin.com/company/" target="_blank" class="social-link">
                                <img src="../assets/images/linkedin.svg" alt="facebook">
                            </a> -->
                            <a href="https://www.instagram.com/airomoni/" target="_blank" class="social-link">
                                <img src="../assets/images/instagram.svg" alt="facebook">
                            </a>
                        </div>
                    </div>
                </div>
                <div class="col s12 copyright-div">
                    <p>
                        © Airopay Ltd. All rights reserved
                    </p>
                    <p>
                        <router-link to="/privacy-policy" tag="a" @click="scrollToTop()" class="sec-color">Privacy Policy</router-link>
                        <span> || </span>
                        <router-link to="/terms" tag="a" @click="scrollToTop()" class="sec-color">Terms of Service</router-link>
                    </p>
                </div>
            </div>
        </div>
    </footer>
</template>

<script>
import M from "materialize-css";
export default {
    name: 'Footer',
    mounted() {
        var elemsScrollspy = document.querySelectorAll('.scrollspy');
        M.ScrollSpy.init(elemsScrollspy);
    },
     methods: { 
        scrollToTop() {
            window.scrollTo(0,0);
        }
    }
}
</script>

<style scoped src="..\assets\css\footer.css"></style>
