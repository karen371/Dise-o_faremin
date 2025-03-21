<script>
export default {
  name: 'Navbar'
}
</script>

<template>
  <!--bg-transparent -->
  <nav class="navbar navbar-expand-lg bg-primary position-fixed w-100">
    <div class="container-fluid">
      <!-- Logo a la izquierda -->
      <a class="navbar-brand text-white" href="#">Navbar</a>

      <!-- Botón de menú en móviles -->
      <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav" 
        aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
        <span class="navbar-toggler-icon"></span>
      </button>

      <!-- Menú de navegación -->
      <div class="collapse navbar-collapse" id="navbarNav">
        <ul class="navbar-nav ms-auto"> <!-- Alinea los ítems a la derecha -->
          <li class="nav-item">
            <a class="nav-link text-white" href="#">Nuestra Empresa</a>
          </li>
          <li class="nav-item">
            <a class="nav-link text-white" href="#">Servicios</a>
          </li>
          <li class="nav-item">
            <a class="nav-link text-white" href="#">Noticias</a>
          </li>
          <li class="nav-item">
            <a class="nav-link text-white" href="#">Trabaja con Nosotros</a>
          </li>
          <li class="nav-item">
            <a class="nav-link text-white" href="#">Contacto</a>
          </li>
          <li class="nav-item">
            <a class="nav-link text-white" href="#">Intranet</a>
          </li>
        </ul>
      </div>
    </div>
  </nav>
</template>

<style scoped>
/* Navbar transparente */
.navbar {
  position: fixed;
  top: 0;
  left: 0;
  right: 0;
  padding: 1rem 2rem;
  background: rgba(0, 0, 0, 0.5); /* Transparente con fondo oscuro */
  backdrop-filter: blur(10px);
  z-index: 1000;
}

/* Estilos de los links */
.nav-link {
  color: white !important;
  transition: background-color 0.3s ease;
  padding: 10px;
  border-radius: 5px;
}

/* Color al hacer hover */
.nav-link:hover {
  background-color: #333333;
}

@media (max-width: 768px) {
  .navbar {
    padding: 0.5rem 1rem;
  }
}
</style>
