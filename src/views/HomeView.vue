<template>
  <div class="home">
    <HelloWorld msg="Welcome to Your Vue.js App"/>
  </div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from '@/components/HelloWorld.vue'

export default {
  name: 'HomeView',
  components: {
    HelloWorld
  },
  created() {
    this.axios.get('https://jsonplaceholder.typicode.com/todos')
      .then(response => {
        console.log(response.data)
      })
      .catch(error => {
        console.log(error)
      })
  },

}
</script>
