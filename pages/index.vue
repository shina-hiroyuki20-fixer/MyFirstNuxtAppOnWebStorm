<template>
  <div>
    <!--    -->
  </div>
</template>

<script lang="ts">
import Vue from 'vue';

export default Vue.extend({
  async mounted () {
    console.log(
      JSON.stringify(await
      this.$axios.$get('https://api.worldoftanks.asia/wot/account/info/?application_id=687e3868f13387ec81f6f7ee8c19376e&account_id=2008482749'), true, '')
    );
  }
});
</script>

<style>
  .container {
    margin: 0 auto;
    min-height: 100vh;
    display: flex;
    justify-content: center;
    align-items: center;
    text-align: center;
  }

  .title {
    font-family: 'Quicksand',
    'Source Sans Pro',
    -apple-system,
    BlinkMacSystemFont,
    'Segoe UI',
    Roboto,
    'Helvetica Neue',
    Arial,
    sans-serif;
    display: block;
    font-weight: 300;
    font-size: 100px;
    color: #35495e;
    letter-spacing: 1px;
  }

  .subtitle {
    font-weight: 300;
    font-size: 42px;
    color: #526488;
    word-spacing: 5px;
    padding-bottom: 15px;
  }

  .links {
    padding-top: 15px;
  }
</style>
