<script>
export default {
  data() {
    return {
      jogadores: [
        { id: 1, name: "Jogador 1", timeid: 1 },
        { id: 2, name: "Jogador 2", timeid: 2 },
        { id: 3, name: "Jogador 3", timeid: 3 },
        { id: 4, name: "Jogador 4", timeid: 4 },
      ],
    };
  },
};
</script>
<template>
  <div class="container">
    <div class="title">
      <h2>Gerenciamento de jogadores</h2>
    </div>
  </div>
  <div class="form-input">
    <input type="text" placeholder="Nome" />
    <input type="text" placeholder="Time" />
    <button>Salvar</button>
  </div>
  <div class="list-items">
    <table>
      <thead>
        <tr>
          <th>ID</th>
          <th>Nome</th>
          <th>Time ID</th>
          <th>Ações</th>
        </tr>
      </thead>
      <tbody>
        <tr v-for="jogador in jogadores" :key="jogador.id">
          <td>{{ jogador.id }}</td>
          <td>{{ jogador.name }}</td>
          <td>{{ jogador.timeid }}</td>
          <td>???</td>
        </tr>
      </tbody>
    </table>
  </div>
</template>

<style scoped></style>
