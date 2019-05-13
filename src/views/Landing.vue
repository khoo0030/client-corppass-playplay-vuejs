<template>
  <div>
    <button @click="login">Go to MockPass</button>
  </div>
</template>

<script>
export default {
  methods: {
    login () {
      location.replace(`${process.env.VUE_APP_SERVICE_PROVIDER_URL}/corppass-login`)
    }
  }
}
</script>
