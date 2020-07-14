<template>
  <div>
    <p>
      User Id: {{userId}}
    </p>
  </div>
</template>

<script>
  export default {
    name: '_id',
    data() {
      return {
        userId: this.$route.params.id
      }
    }
  }
</script>

<style scoped>

</style>
