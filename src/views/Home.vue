<template>
  <div class="home">
    <button @click="login">Login to Corp Pass</button>
  </div>
</template>

<script>
// @ is an alias to /src
import axios from 'axios'

export default {
  methods: {
    async login () {
      try {
        const response = await axios.get('http://localhost:7002')
        console.log(response)
      } catch (e) {
        console.error(e)
      }
    }
  }
}
</script>
