<template>
  <header class="menu-superior">
    <div class="menu-esquerdo">
      <span> Home </span>
      <span>|</span>
      <span> Times </span>
      <span>|</span>
      <span> Jogadores </span>
    </div>
    <div class="menu-direito">
      <span>Sair</span>
    </div>
  </header>
  <RouterView />
</template>

<style>
@import "@/assets/base.css";

#app {
  max-width: 1280px;
  margin: 0 auto;
  /* padding: 2rem; */
  font-weight: normal;
  height: 100vh;
}

header,
footer {
  background-color: rgb(100, 50, 150);
  color: white;
  height: 15%;
  font-size: 1.3rem;
  display: flex;
  align-items: center;
  padding-left: 2rem;
}

header span {
  padding: 0 20px;
}

.menu-superior {
  justify-content: space-between;
}

main {
  height: 70%;
}
</style>
