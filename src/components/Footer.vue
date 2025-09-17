<template>
  <footer class="footer">
    <div class="container">
      <!-- Acerca -->
      <div class="column">
        <h3 class="title">ACERCA</h3>
        <p>
          En La Escuela Especializada en Ingeniería ITCA-FEPADE estamos
          comprometidos con la calidad académica, la empresarialidad y la
          pertinencia de nuestra oferta educativa.
        </p>
        <div class="social-icons">
          <a href="#" aria-label="YouTube"><i class="fab fa-youtube"></i></a>
          <a href="#" aria-label="Facebook"><i class="fab fa-facebook"></i></a>
          <a href="#" aria-label="Twitter"><i class="fab fa-twitter"></i></a>
          <a href="#" aria-label="Instagram"><i class="fab fa-instagram"></i></a>
        </div>
      </div>

      <!-- Institución -->
      <div class="column">
        <h3 class="title">INSTITUCIÓN</h3>
        <ul>
          <li><a href="#">Cooperación Nacional e Internacional</a></li>
          <li><a href="#">Gestión de la Calidad</a></li>
          <li><a href="#">Investigación y Proyección Social</a></li>
          <li><a href="#">Publicaciones</a></li>
          <li><a href="#">Buzón de Sugerencias, Quejas y Reclamos</a></li>
        </ul>
      </div>

      <!-- Cursos -->
      <div class="column">
        <h3 class="title">CURSOS</h3>
        <ul>
          <li><a href="#">Academia CISCO</a></li>
          <li><a href="#">Gastronomía</a></li>
          <li><a href="#">Mecatrónica, Electrónica e Industria 4.0</a></li>
          <li><a href="#">Idiomas</a></li>
          <li><a href="#">Tecnologías Informáticas</a></li>
          <li><a href="#">Eléctrica, Automotriz, Mecánica Industrial, Civil y Construcción</a></li>
        </ul>
      </div>

      <!-- Carreras -->
      <div class="column">
        <h3 class="title">CARRERAS</h3>
        <ul>
          <li><a href="#">Sede Santa Tecla</a></li>
          <li><a href="#">Regional La Unión</a></li>
          <li><a href="#">Regional San Miguel</a></li>
          <li><a href="#">Regional Santa Ana</a></li>
          <li><a href="#">Regional Zacatecoluca</a></li>
        </ul>
      </div>
    </div>
  </footer>
</template>

<script>
export default {
  name: "Footer",
};
</script>

<style scoped>
.footer {
  background-color: #d6bb7b; /* Color similar al de tu imagen */
  padding: 3rem 2rem;
  color: #1a1a1a;
}

.container {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(220px, 1fr));
  gap: 2rem;
  max-width: 1200px;
  margin: 0 auto;
}

.column .title {
  font-size: 1rem;
  font-weight: bold;
  letter-spacing: 1px;
  margin-bottom: 0.8rem;
  text-transform: uppercase;
  position: relative;
  color: #2b2b2b;
}

.column .title::after {
  content: "";
  display: block;
  width: 40px;
  height: 2px;
  background: #8b2d2d; /* Rojo vino */
  margin-top: 0.3rem;
}

.column p {
  font-size: 0.95rem;
  line-height: 1.6;
}

.column ul {
  list-style: none;
  padding: 0;
}

.column ul li {
  margin-bottom: 0.5rem;
}

.column ul li a {
  text-decoration: none;
  color: #1a1a1a;
  font-size: 0.95rem;
  transition: color 0.2s ease;
}

.column ul li a:hover {
  color: #8b2d2d; /* Hover en rojo */
}

.social-icons {
  margin-top: 1rem;
}

.social-icons a {
  margin-right: 10px;
  font-size: 1.2rem;
  color: #1a1a1a;
  transition: color 0.3s ease;
}

.social-icons a:hover {
  color: #8b2d2d;
}
</style>
