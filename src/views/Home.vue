<template>
  <div class="home">
    <div class="jumbotron">
      <h1 class="display-4">Esercizio Vue.js</h1>
      <p class="lead">
        Questo è un progetto di prova per prendere dimestichezza con Vue, Axios
        e una libreria di componenti come Element. Per iniziare visualizza le
        istruzioni
      </p>
      <router-link to="/istruzioni"
        ><el-button type="primary">Vai alle istruzioni</el-button></router-link
      >
      <h3 class="mt-4">Moduli pre-installati</h3>
      <ul>
        <li>
          <a href="https://getbootstrap.com/" target="_blank">Bootstrap</a>
        </li>
        <li><a href="https://lodash.com/" target="_blank">Lodash</a></li>
        <li><a href="https://lodash.com/">Element-ui</a></li>
      </ul>
    </div>
  </div>
</template>

<script>
export default {
  name: "Home"
};
</script>
