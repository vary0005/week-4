<template>
  <div id="app">
    <div>
      <el-button @click="openDiag = true" type="primary">Welcome</el-button>
      <el-dialog :visible.sync="openDiag">
        <div>
          <input type="text" v-model="sendTreat">
        </div>
        <HelloWorld msg="Welcome to Your Vue.js App"/>
        <NewMessage :treat="SendTreat"/>
      </el-dialog>
    </div>
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue';

export default {
  name: 'app',
  components: {
    HelloWorld,
  },
  data() {
    return {
      openDiag: false,
    };
  },
};
</script>

<style>
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
