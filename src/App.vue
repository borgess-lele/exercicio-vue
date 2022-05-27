<script>
import { RouterLink, RouterView } from "vue-router";

export default {
  components: { RouterLink, RouterView },
};
</script>

<template>
  <header>
    <div class="wrapper">
      <nav>
        <RouterLink to="/">Home</RouterLink>
        <RouterLink to="/about">About</RouterLink>
        <RouterLink to="/alunos">Alunos</RouterLink>
      </nav>
    </div>
  </header>

  <main>
    Parte fixa...
    <RouterView />
  </main>

  <footer>ajhghajhdsjdshbjcshkisabab</footer>
</template>

<style>
@import "@/asstes/base.css";

#app {
  max-width: 1280px;
  margin: 0 auto;
  padding: 2rem;

  font-weight: normal;
  height: 100vh;
}

header {
  border: 1px solid black;
}

footer {
  border: 1 px solid black;
}

main {
  border: 1px solid black;
  margin-top: 3%;
  margin-bottom: 3%;
  height: 80%;
}

a,
.green {
  text-decoration: none;
  color: hsla(160, 100%, 37%, 1);
  transition: 0.4s;
}

@media (hover: hover) {
  a:hover {
    background-color: hsla(160, 100%, 37%, 0.2);
  }
}

nav {
  width: 100%;
  font-size: 12px;
  text-align: center;
  margin-top: 2rem;
}

nav a.router-link-exact-active {
  color: var(--color-test);
}

nav a.router-link-exact-active:hover {
  background-color: transparent;
}

nav a {
  display: inline-block;
  padding: 0 1rem;
  border-left: 1px solid var(--color-border);
}

nav a:first-of-type {
  border: 0;
}
</style>
