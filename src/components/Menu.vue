<template>
  <nav class="top-menu">
    <div class="container">
      <ul class="nav">
        <li v-for="item in menu" :key="item.id" class="menu-item" :class="{ dropdown: item.children && item.children.length }">
          <a 
            :href="item.link || '#'" 
            @click.prevent="toggleDropdown(item)" 
            class="menu-link"
          >
            {{ item.name }}
            <span v-if="item.children" class="caret">▼</span>
          </a>
          <ul v-if="item.children && item.show" class="dropdown-menu">
            <li v-for="child in item.children" :key="child.id" class="menu-item">
              <a :href="child.link || '#'">{{ child.name }}</a>
            </li>
          </ul>
        </li>
      </ul>
    </div>
  </nav>
</template>

<script>
export default {
  data() {
    return {
      menu: [
        {
          id: 1,
          name: "Institución",
          children: [
            { id: 11, name: "Quiénes Somos", link: "#" },
            { id: 12, name: "Premios y reconocimientos", link: "#" },
            { id: 13, name: "Organigrama", link: "#" },
            { id: 14, name: "Cooperación Nacional e Internacional", link: "#" }
          ],
          show: false
        },
        { id: 2, name: "Carreras", link: "#" },
        { id: 3, name: "Nuevo Ingreso", link: "#" },
        { id: 4, name: "Cursos y Diplomados", link: "#" },
        { id: 5, name: "Investigación y Proyección Social", link: "#" },
        {
          id: 6,
          name: "Recursos Estudiantiles",
          children: [
            { id: 61, name: "Portal", link: "#" },
            { id: 62, name: "Biblioteca", link: "#" }
          ],
          show: false
        },
        {
          id: 7,
          name: "Noticias",
          children: [
            { id: 71, name: "Noticias", link: "#" }
          ],
          show: false
        },
        {
          id: 8,
          name: "Contáctenos",
          children: [
            { id: 81, name: "Directorio", link: "#" },
            { id: 82, name: "Carreras técnicas e ingenierías", link: "#" }
          ],
          show: false
        },
        {
          id: 9,
          name: "Mesón de Goya",
          children: [
            { id: 91, name: "Nosotros", link: "#" },
            { id: 92, name: "Servicios", link: "#" },
            { id: 93, name: "Historia", link: "#" }
          ],
          show: false
        }
      ]
    };
  },
  methods: {
    toggleDropdown(item) {
      if (item.children) {
        item.show = !item.show;
      }
    }
  }
};
</script>

<style scoped>
.top-menu {
  background: linear-gradient(to bottom, #d8a239, #c78e27);
  padding: 0.5rem 0;
  font-family: Arial, sans-serif;
}

.nav {
  display: flex;
  list-style: none;
  padding: 0;
  margin: 0;
}

.menu-item {
  position: relative;
  margin-right: 1rem;
}

.menu-link {
  color: white;
  text-decoration: none;
  padding: 0.5rem 1rem;
  display: block;
}

.menu-link:hover {
  background-color: rgba(255,255,255,0.2);
}

.caret {
  margin-left: 0.25rem;
  font-size: 0.6rem;
}

.dropdown-menu {
  position: absolute;
  top: 100%;
  left: 0;
  background: #fff;
  list-style: none;
  padding: 0.5rem 0;
  margin: 0;
  min-width: 200px;
  box-shadow: 0 4px 6px rgba(0,0,0,0.1);
  z-index: 10;
}

.dropdown-menu .menu-item a {
  color: #333;
  padding: 0.5rem 1rem;
  display: block;
}

.dropdown-menu .menu-item a:hover {
  background-color: #f0f0f0;
}
</style>
