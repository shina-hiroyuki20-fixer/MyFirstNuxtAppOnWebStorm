<template>
  <div>
    <p>
      User Id: {{ userId }}
    </p>
  </div>
</template>

<script lang="ts">
import Vue from 'vue';

export default Vue.extend({
  data (): { userId: string } {
    return {
      userId: this.$route.params.id
    };
  }
});
</script>

<style scoped>

</style>
