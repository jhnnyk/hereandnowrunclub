<script setup></script>

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
</style>
