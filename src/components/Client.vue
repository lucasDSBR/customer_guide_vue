<!-- eslint-disable vue/multi-word-component-names -->
<!-- eslint-disable vue/no-dupe-keys -->
<template>
  <div class="hello">
	<h4>{{name}}</h4>
	<button @click="mudarCor">Mudar Cor!</button>
  </div>
</template>

<script>
export default {

  // eslint-disable-next-line vue/multi-word-component-names
  name: 'Client',
  data() {
	return {
		name: "Lucas",
		description: "sadasdkajld",
		isPremium: false
	}
  },
  props: {
	// eslint-disable-next-line vue/no-dupe-keys
	msg: String,
	showText: Boolean,
	// eslint-disable-next-line vue/no-dupe-keys
	name: String,
	totSallers: Number
  },
  methods: {
	mudarCor: function(){
		alert("Chamour")
	}
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}

.client-premium {
	color: red;
}

.client {
	color: green;
}
</style>
