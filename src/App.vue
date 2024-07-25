<template>
  <div id="app">
    <table>
      <thead>
        <tr>
          <th>Código</th>
          <th>Nombre</th>
          <th>Stock</th>
          <th>Precio</th>
          <th>Incrementar o decrementar</th>
       
        </tr>
      </thead>
      <tbody>
        <tr v-for="game in games" :key="game.codigo">
          <td>{{ game.codigo }}</td>
          <td>{{ game.nombre }}</td>
          <td>{{ game.stock }}</td>
          <td>{{ game.precio }}</td>
          
          <td>
            <button @click="decrementStock(game.codigo)">-</button>
            <button @click="incrementStock(game.codigo)">+</button>
          </td>
        </tr>
      </tbody>
    </table>
  </div>
</template>

<script>
import { mapState, mapActions } from 'vuex';

export default {
  name: 'App',
  computed: {
    ...mapState({
      games: (["games"]),
    }),
  },
  methods: {
    ...mapActions(['incrementStock', 'decrementStock']),
  },
};
</script>

<style>
table {
  width: 100%;
  border-collapse: collapse;
}

th, td {
  border: 1px solid #ddd;
  padding: 8px;
}

th {
  background-color: #f2f2f2;
}

button {
  margin: 0 5px;
  padding: 5px 10px;
}
</style>
