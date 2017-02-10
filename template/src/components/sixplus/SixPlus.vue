<template>
  <div class="sixplus">
    <div class="logo">
      <img src="/static/img/LOGO_SIXPLUS.svg">
    </div>
    <h1><a :href="url" target="_blank">{{ title }}</a></h1>
    <p>{{ chapo }}</p>
    <hr>
    <pre>{{ version }}</pre>
  </div>
</template>

<script>
  export default {
    data () {
      return {
        title: 'Six Plus',
        url: 'http://www.liberation.fr/data-nouveaux-formats-six-plus,100538',
        chapo: 'Un boilerplate Vue.js pour Libération Six Plus basé sur vue-webpack',
        version: '1.0.0'
      }
    }
  }
</script>

<style>
  .sixplus {max-width: 960px; margin: 3em auto; padding: 1em; text-align: center; background: #fff; border: 1px solid #dedede;}
  .sixplus .logo {max-width: 160px; margin: 0 auto;}
  .sixplus h1 {font-family: 'libesansweb-semicondensed'; letter-spacing: .06em;}
</style>
