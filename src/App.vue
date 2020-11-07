<template>
  <div id="nav">
    <router-link to="/">Home</router-link> |
    <router-link to="/about">About</router-link>
  </div>
  <router-view/>
</template>

<script>
import { onMounted } from 'vue';
import HelloWorld from './components/HelloWorld.vue';

export default ({
  setup() {
    const greet = async () => {
      const wasm = import('../wasm/pkg');
      const greet = (await wasm).greet;
      const t = greet('Rust');
      console.log(t);
    };
    onMounted(() => {
      greet();
    });
  },
});
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

#nav {
  padding: 30px;
}

#nav a {
  font-weight: bold;
  color: #2c3e50;
}

#nav a.router-link-exact-active {
  color: #42b983;
}
</style>
