<script setup>
import { ref } from 'vue';
const showMobileNav = ref(false);
</script>

<template>
  <header>
    <RouterLink to="/">
      <img
        src="../assets/images/logo.png"
        alt="Here and Now Run Club"
        id="logo"
      />
    </RouterLink>

    <nav>
      <RouterLink to="/">Home</RouterLink>
      <RouterLink to="/coaches">Coaches</RouterLink>
    </nav>

    <div class="social">
      <a href="https://www.strava.com/clubs/hereandnow" target="_blank">
        <img src="../assets/images/strava.png" alt="Here & Now on Strava" />
      </a>

      <a href="https://www.instagram.com/hereandnowruncrew/" target="_blank">
        <img src="../assets/images/ig.png" alt="Here & Now on Instagram" />
      </a>
    </div>

    <div
      class="mobile-menu"
      @click="showMobileNav = !showMobileNav"
      :class="{ close: showMobileNav }"
    >
      <div class="bar1"></div>
      <div class="bar2"></div>
      <div class="bar3"></div>
    </div>

    <ul class="mobile-nav" v-if="showMobileNav">
      <li><RouterLink to="/">Home</RouterLink></li>
      <li><RouterLink to="/coaches">Coaches</RouterLink></li>
      <li class="mobile-socials">
        <a href="https://www.strava.com/clubs/hereandnow" target="_blank">
          <img src="../assets/images/strava.png" alt="Here & Now on Strava" />
        </a>

        <a href="https://www.instagram.com/hereandnowruncrew/" target="_blank">
          <img src="../assets/images/ig.png" alt="Here & Now on Instagram" />
        </a>
      </li>
    </ul>
  </header>
</template>

<style>
header {
  background: url('../assets/images/DSC02505.jpg') no-repeat center 85%;
  background-size: cover;
  padding: 2% 2% 12% 2%;
  display: flex;
  justify-content: space-between;
  font-size: 1.2em;
}

header a {
  color: white;
  padding: 0 12px;
  font-weight: bold;
  text-decoration: none;
}

header a:hover {
  text-decoration: underline;
}

#logo {
  width: 230px;
  height: 230px;
}

.mobile-menu {
  display: none;
}

.mobile-menu div {
  width: 35px;
  height: 5px;
  background-color: white;
  margin: 6px 0;
  border-radius: 2px;
  transition: 0.4s;
}

.close .bar1 {
  -webkit-transform: rotate(-45deg) translate(-9px, 7px);
  transform: rotate(-45deg) translate(-9px, 7px);
}

.close .bar2 {
  opacity: 0;
}

.close .bar3 {
  -webkit-transform: rotate(45deg) translate(-8px, -7px);
  transform: rotate(45deg) translate(-8px, -7px);
}

@media (max-width: 600px) {
  #logo {
    width: 140px;
    height: 140px;
  }

  .mobile-menu {
    display: block;
    margin-right: 10px;
  }

  nav,
  .social {
    display: none;
  }
}

.mobile-nav {
  position: absolute;
  top: 45px;
  right: 10px;
  margin: 0;
  padding: 0;
  text-align: right;
  /* background: rgba(2, 2, 2, 0.5); */
  border-radius: 10px;
}

.mobile-nav li {
  list-style-type: none;
  margin: 0;
  padding: 5px;
  border-bottom: 1px solid black;
}

.mobile-nav li.mobile-socials {
  padding-top: 10px;
}
</style>
