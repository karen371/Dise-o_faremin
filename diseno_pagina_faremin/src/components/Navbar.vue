<script>
export default {
    name: 'Navbar'
}
</script>

<template>
    <nav>
        <nav class="navbar">
            <div class="navbar-brand">
              <img src="" alt="Logo" class="logo">
            </div>
            <div class="navbar-menu">
              <router-link to="/" class="nav-item text-light font-light">Nuesta Empresa</router-link>
              <router-link to="/" class="nav-item text-light font-light">Servicios</router-link>
              <router-link to="/" class="nav-item text-light font-light">Noticias</router-link>
              <router-link to="/" class="nav-item  text-light font-light">Trabaja con Nosotros</router-link>
              <router-link to="/" class="nav-item text-light font-light">Contacto</router-link>
              <router-link to="/" class="nav-item text-light font-light">Intranet</router-link>
            </div>
          </nav>
    </nav>
</template>
<style scoped>
.navbar {
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 1rem 2rem;
  position: fixed;
  top: 0;
  left: 0;
  right: 0;
  background: rgba(174, 25, 25, 0.9);
  backdrop-filter: blur(10px);
  z-index: 1000;
}

.navbar-brand {
  display: flex;
  align-items: center;
}

.logo {
  height: 40px;
  width: auto;
}

.navbar-menu {
  display: flex;
  gap: 2rem;
  margin-right: 15px;
}

.nav-item {
  text-decoration: none;
  font-weight: 500;
  transition: color 0.3s ease;
  font-size: 1rem;
  border-radius: 5px;
  padding: 10px;
}

.nav-item:hover {
  background-color: var(--detail-dark);
}

@media (max-width: 768px) {
  .navbar-menu {
    display: none;
  }
}
</style>