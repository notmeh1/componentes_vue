<template>
  <div class="container">
    <ul>
      <li v-for="(personaje, index) in personajes" :key="index" class="card_list">
        <img :src="personaje.src" alt="" class="card_img"/>
        <h1 class="card_name">{{personaje.nombre}}</h1>
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  name: "Personajes",
  data: () => ({
    personajes: [
      {
        nombre: "Rick Sanchez",
        src: "https://rickandmortyapi.com/api/character/avatar/1.jpeg",
      },
      {
        nombre: "Morty Smith",
        src: "https://rickandmortyapi.com/api/character/avatar/2.jpeg",
      },
    ],
  }),
};
</script>

<style lang="scss">
.container {
  display: flex;
}
.card_list {
  flex-direction: column;
}
.card_img {
  border-radius: 150px;
}
.card_name {
  text-align: center;
  color: #ffffff;
}
</style>
