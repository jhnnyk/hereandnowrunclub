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
  </header>
</template>

<style>
header {
  background: url('../assets/images/DSC02505.jpg') no-repeat center 85%;
  background-size: cover;
  padding: 2% 2% 12% 2%;
  display: flex;
  justify-content: space-between;
}

header a {
  color: white;
  padding: 0 10px;
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
