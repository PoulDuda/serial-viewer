<template>
  <div id="app">
    <Header />
    <router-view />
  </div>
</template>

<script>
import Header from './components/Header.vue';

export default {
  name: 'App',
  components: {
    Header
  }
};
</script>

<style>
/* Здесь можно добавить глобальные стили */
main {
  padding-top: 4rem; /* Отступ, чтобы контент не перекрывался хедером */
}
</style>
