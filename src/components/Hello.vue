<template>
  <div class="hello">
    <h1>{{ msg }}</h1>

  </div>
</template>

<script>
import store from '../vuex'

export default {
  name: 'hello',
  data () {
    return {
      msg: 'Welcome to My Vue.js App, My name is Tamir Amid'
    }
  },
  mounted: function () {
    store.commit('pageLoaded', 'hello')
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1, h2 {
  font-weight: normal;
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
</style>
