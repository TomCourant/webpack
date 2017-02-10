<template>
  <div id="app">
    {{#router}}
    <router-view></router-view>
    {{else}}
    <sixPlus></sixPlus>
    {{/router}}
  </div>
</template>

<script>
{{#unless router}}
import SixPlus from './components/sixplus/SixPlus'{{#if_eq lintConfig "airbnb"}};{{/if_eq}}

{{/unless}}
export default {
  name: 'app'{{#router}}{{#if_eq lintConfig "airbnb"}},{{/if_eq}}{{else}},
  components: {
    SixPlus{{#if_eq lintConfig "airbnb"}},{{/if_eq}}
  }{{#if_eq lintConfig "airbnb"}},{{/if_eq}}{{/router}}
}{{#if_eq lintConfig "airbnb"}};{{/if_eq}}
</script>

<style src="./app.css"></style>
