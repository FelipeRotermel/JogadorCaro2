<template>
  <header>Cabeçalho</header>
  <main>Main</main>
  <footer>Footer</footer>
</template>

<style>
@import '@/assets/base.css';

#app {
  max-width: 1280px;
  margin: 0 auto;
  /* padding: 2rem; */
  font-weight: normal;
  height: 100vh;
}

header, footer {
  background-color: rgb(100,50,150);
  color: white;
  height: 15%;
  font-size: 1.3rem;
  display: flex;
  align-items: center;
  padding-left: 2rem;
}

main {
  height: 70%;
}

</style>
