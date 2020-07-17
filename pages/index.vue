<template>
  <div>
    <!--    -->
  </div>
</template>

<script lang="ts">
import Vue from 'vue';
import { NuxtAxiosInstance } from '@nuxtjs/axios';

export default Vue.extend({
  async asyncData ({ $axios }: { $axios: NuxtAxiosInstance }) { // 1a99d197-32f1-4c78-8591-85b3232db99f
    console.log(
      JSON.stringify(await
      $axios.$get('https://atnd.ak4.jp/api/cooperation/FIXER2018/staffs/193491?token=1a99d197-32f1-4c78-8591-85b3232db99f'))
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
