<template>
  <div class="page-container">
    <!-- Encabezado -->
    <header class="header">
      <h1 class="title">ITCA-FEPADE</h1>
      <p class="subtitle">Instituto Tecnológico Centroamericano</p>
    </header>

    <!-- ¿Quiénes somos? -->
    <section class="about-box">
      <h2 class="section-title">¿QUIÉNES SOMOS?</h2>
      <p class="section-text">
        El Instituto Tecnológico Centroamericano (ITCA-FEPADE) es una institución de
        educación superior especializada en la formación tecnológica. Brinda carreras
        técnicas, ingenierías y programas de educación continua, enfocados en la práctica
        y en las demandas del mercado laboral.
      </p>
    </section>

    <!-- Misión, visión y valores -->
    <section class="info-box">
      <div class="mv-container">
        <div class="section">
          <h2 class="section-title">MISIÓN</h2>
          <p class="section-text">
            Formar profesionales integrales y competentes en las áreas
            tecnológicas que tengan demanda y oportunidad en el mercado local,
            regional y mundial tanto como trabajadores y como empresarios.
          </p>
        </div>

        <div class="section">
          <h2 class="section-title">VISIÓN</h2>
          <p class="section-text">
            Ser una institución educativa líder en educación tecnológica a nivel
            nacional y regional, comprometida con la calidad, la empresarialidad
            y la pertinencia de nuestra oferta educativa.
          </p>
        </div>
      </div>

      <div class="section valores">
        <h2 class="section-title">VALORES</h2>
        <p class="section-text">
          Excelencia, Integridad, Espiritualidad, Cooperación y Comunicación.
        </p>
      </div>
    </section>
  </div>
</template>

<script>
export default {
  name: "CuerpoPaginaItca",
};
</script>

<style scoped>
.page-container {
  background: #f9fafb;
  min-height: 100vh;
  padding: 2rem;
  font-family: "Segoe UI", Tahoma, Geneva, Verdana, sans-serif;
}

/* Encabezado */
.header {
  text-align: center;
  margin-bottom: 2.5rem;
}
.title {
  font-size: 2.5rem;
  font-weight: bold;
  color: #e00b24; /* Azul fuerte */
}
.subtitle {
  font-size: 1.2rem;
  color: #111111; /* Gris */
  margin-top: 0.5rem;
}

/* ¿Quiénes somos? */
.about-box {
  max-width: 850px;
  margin: 0 auto 3rem auto;
  background: #fff;
  border-radius: 1rem;
  padding: 2rem;
  box-shadow: 0 4px 10px rgba(0, 0, 0, 0.1);
  text-align: center;
}
.about-box .section-title {
  color: #161616; /* Azul brillante */
}
.about-box .section-text {
  color: #0f0f10; /* Gris oscuro */
  line-height: 1.6;
}

/* Caja misión, visión y valores */
.info-box {
  background: #cc8a10; /* Dorado */
  color: white;
  border-bottom: 4px solid #a11d1d; /* Línea roja */
  border-radius: 0.5rem 0.5rem 0 0;
  padding: 3rem 2rem;
  text-align: center;
}

.mv-container {
  display: flex;
  flex-direction: column;
  gap: 2.5rem;
  margin-bottom: 2.5rem;
}

@media (min-width: 768px) {
  .mv-container {
    flex-direction: row;
    justify-content: space-around;
    text-align: center;
  }
  .mv-container .section {
    flex: 1;
    padding: 0 1rem;
  }
}

.section-title {
  font-size: 1.5rem;
  font-weight: bold;
  margin-bottom: 1rem;
}

.section-text {
  font-size: 1rem;
  line-height: 1.6;
}

.valores {
  margin-top: 2rem;
}
</style>

