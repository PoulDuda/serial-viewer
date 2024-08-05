<template>
  <footer>
    <div class="footer-content">
      <div class="logo-container">
        <img :src="logoUrl" alt="Logo" class="logo" />
      </div>
      <p>&copy; 2024 PoulDudaa. All rights reserved.</p>
    </div>
  </footer>
</template>

<script>
export default {
  name: 'Footer',
  data() {
    return {
      logoUrl: 'footer.png'
    };
  }
};
</script>

<style scoped>
footer {
  background-color: white;
  color: black;
  padding: 2rem;
  text-align: center;
}

.footer-content {
  display: flex;
  flex-direction: column;
  align-items: center;
}

.logo-container {
  margin-bottom: 1rem;
}

.logo {
  max-height: 50px;
  width: auto;
}

nav ul {
  list-style: none;
  display: flex;
  gap: 2rem;
  margin: 1rem 0;
  padding: 0;
}

.nav-icon {
  max-height: 30px;
  width: auto;
}

nav a:hover {
  text-decoration: underline;
}

p {
  margin-top: 1rem;
  font-size: 1rem;
}

@media (max-width: 600px) {
  .logo {
    max-height: 40px;
  }

  .nav-icon {
    max-height: 25px;
  }

  nav ul {
    gap: 1rem;
  }
}
</style>
