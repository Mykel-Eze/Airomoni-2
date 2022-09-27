<template>
  <div>
    <nav class="trans-nav">
        <div class="container">
            <div class="nav-wrapper">
                <router-link to="/" class="brand-logo">
                    <img src="../assets/images/logo.svg" alt="Airomoni" class="logo">
                </router-link>

                <ul id="nav-mobile" class="right hide-on-med-and-down ul-nav">
                    <li>
                        <a href="/#sect-1" class="">About</a>
                    </li>
                    <li>
                        <router-link to="/faq" class="">FAQ</router-link>
                    </li>
                    <li>
                        <a href="#footer" class="">Contact</a>
                    </li>
                    <li class="unknown-device rel">
                        <button class="nav-pry-btn-2 btn pointer unknown-device-btn">Download Now</button>
                        <div class="flex-div abs-btn-wrapper">
                            <button class="btn app-store google-store" style="margin-right: 10px" onclick="window.location.href='https://play.google.com/store/apps/details?id=com.airopay.agents&hl=en&gl=US'">
                                <img src="../assets/images/google-btn.svg" alt="play store">
                            </button>
                            <button class="btn app-store apple-store">
                                <img src="../assets/images/apple-btn.svg" alt="apple store" onclick="window.location.href='https://apps.apple.com/tt/app/airomoni/id1560560802'">
                            </button>
                        </div>
                    </li>
                    <li class="andriod-device">
                        <button class="btn app-store google-store" onclick="window.location.href='https://play.google.com/store/apps/details?id=com.airopay.agents&hl=en&gl=US'">
                            <img src="../assets/images/google-btn.svg" alt="play store">
                        </button>
                    </li>
                    <li class="ios-device">
                        <button class="btn app-store apple-store" onclick="window.location.href='https://apps.apple.com/tt/app/airomoni/id1560560802'">
                            <img src="../assets/images/apple-btn.svg" alt="apple store">
                        </button>
                    </li>
                </ul>
                <ul class="right dn-mobile ul-nav">
                    <li class="unknown-device rel">
                        <button class="nav-pry-btn-2 btn pointer unknown-device-btn">Download Now</button>
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
                        <button class="btn app-store google-store" onclick="window.location.href='https://play.google.com/store/apps/details?id=com.airopay.agents&hl=en&gl=US'">
                            <img src="../assets/images/google-btn.svg" alt="play store">
                        </button>
                    </li>
                    <li class="ios-device">
                        <button class="btn app-store apple-store" onclick="window.location.href='https://apps.apple.com/tt/app/airomoni/id1560560802'">
                            <img src="../assets/images/apple-btn.svg" alt="apple store">
                        </button>
                    </li>
                </ul>
              </div>
        </div>
    </nav>

  </div>
</template>

<script>
// import M from "materialize-css";
// import $ from "jquery";
export default {
  name: "Navbar"
};
</script>

<style scoped src="..\assets\css\navbar.css"></style>
