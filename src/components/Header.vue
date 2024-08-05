<template>
  <header>
    <img :src="logoUrl" alt="Logo" class="Logo">
    <nav>
      <ul>
        <li><a href="#"><img :src="seasonsUrl" alt="Seasons" class="nav-icon" /></a></li>
        <li><a href="#"><img :src="aboutUrl" alt="About" class="nav-icon" /></a></li>
      </ul>
    </nav>
  </header>
</template>

<script>
export default  {
  name: 'Header',
  data(){
    return {
      logoUrl: 'logo.svg',
      aboutUrl: 'about.png',
      seasonsUrl: 'seasons.png'
    };
  }
};
</script>

<style scoped>
header {
  display: flex;
  align-items: center;
  justify-content: space-between;
  padding: 1rem 2rem;
  background-color: white;
  color: white;
  position: fixed;
  width: 90%;
  top: 0;
  left: 0;
  z-index: 1000;
}

.Logo {
  max-height: 60px;
  width: auto;
}

.nav-icon{
  max-height: 20px;
  width: auto;

}

nav ul {
  list-style: none;
  display: flex;
  gap: 3.5rem;
  margin: 0;
  padding: 0;
}

nav a {
  color: black;
  text-decoration: none;
}

nav a:hover {
  text-decoration: underline;
}

@media (max-width: 600px) {
  .Logo {
    max-height: 40px;
  }

  .nav-icon {
    max-height: 25px;
  }

  nav ul {
    list-style: none;
    display: flex;
    gap: 2.5rem;
    margin: 0;
    padding: 0;
  }
}
</style>