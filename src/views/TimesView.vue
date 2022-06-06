<template>
  <div class="container">
    <div class="title">
      <h2>Gerenciamento de times</h2>
    </div>
  </div>
  <div class="form-input">
    <input type="text" />
    <button>Salvar</button>
  </div>
  <div class="list-times">
    <table>
      <thead>
        <tr>
          <th>ID</th>
          <th>Nome</th>
          <th>Ações</th>
        </tr>
      </thead>
      <tbody>
        <tr>
          <th>1</th>
          <th>Time 1</th>
          <th>???</th>
        </tr>
        <tr>
          <th>2</th>
          <th>Time 2</th>
          <th>???</th>
        </tr>
        <tr>
          <th>3</th>
          <th>Time 3</th>
          <th>???</th>
        </tr>
      </tbody>
    </table>
  </div>
</template>

<style>
.title {
  text-align: center;
  margin: 2rem 0;
}

.form-input {
  display: flex;
  justify-content: center;
}

.form-input input {
  width: 50%;
  border: 1px solid #ccc;
  border-radius: 10px;
  padding: 0 1rem;
  height: 40px;
}

.form-input button {
  height: 40px;
  margin-left: 1%;
  background-color: rgb(100, 50, 150);
  font-weight: bold;
  color: white;
  border: 1px solid rgb(100, 50, 150);
  border-radius: 10px;
  width: 15%;
}

.list-times {
  display: flex;
  justify-content: center;
  margin: 2rem 0;
}

table {
  width: 40%;
  border: 1px solid black;
  border-collapse: collapse;
  text-align: center;
}

table thead {
  background-color: rgb(100, 50, 150);
  color: white;
}

table thead th {
  font-weight: bolder;
}

table tbody tr:nth-child(odd) {
  background-color: rgba(100, 50, 150, 0.389);
}
</style>
