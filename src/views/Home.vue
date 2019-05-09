<template>
  <div>
    <button @click="login">Go to MockPass</button>
  </div>
</template>

<script>
export default {
  methods: {
    login () {
      location.replace('http://localhost:7002/corppass-login')
    }
  }
}
</script>
