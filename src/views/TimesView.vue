<script>
import { v4 as uuid } from "uuid";
export default {
  data() {
    return {
      novo_time: "",
      times: [
        { id: "759b5c49-db71-4d82-b199-7a5abd2c4f5b", name: "Time 1" },
        { id: "209c1c2b-6d24-410b-9fca-f03379dcf437", name: "Time 2" },
        { id: "52f38a69-0bf0-45b4-bfad-5a6a96676632", name: "Time 3" },
        { id: "1d7ad795-1952-4a2a-a350-6a8293b1ad7c", name: "Time 4" },
      ],
    };
  },
  methods: {
    salvar() {
      const novo_id = uuid();
      this.times.push({
        id: novo_id,
        name: this.novo_time,
      });
    },
  },
};
</script>
<template>
  <div class="container">
    <div class="title">
      <h2>Gerenciamento de times</h2>
    </div>
  </div>
  <div class="form-input">
    <input type="text" v-model="novo_time" />
    <button @click="salvar">Salvar</button>
  </div>
  <div class="list-items">
    <table>
      <thead>
        <tr>
          <th>ID</th>
          <th>Nome</th>
          <th>Ações</th>
        </tr>
      </thead>
      <tbody>
        <tr v-for="time in times" :key="time.id">
          <td>{{ time.id }}</td>
          <td>{{ time.name }}</td>
          <td>???</td>
        </tr>
      </tbody>
    </table>
  </div>
</template>

<style></style>
