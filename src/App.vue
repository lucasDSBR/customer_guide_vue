<template>
  <img alt="Vue logo" src="./assets/logo.png">
  <HelloWorld msg="Welcome to Your Vue.js App"/>
  <div v-for="client in clients" :key="client.id">
	<Client :name="client.name" :totSallers="client.totSallers"/>
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'
import Client from './components/Client.vue';
export default {
  name: 'App',
  components: {
    HelloWorld,
	Client
  },
  data(){
	return {
		clients: [
			{ id: 1, name: "client 1", totSallers: 2},
			{ id: 2, name: "client 2", totSallers: 4},
			{ id: 3, name: "client 3", totSallers: 5}
		]
	}
  }

}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}


</style>
