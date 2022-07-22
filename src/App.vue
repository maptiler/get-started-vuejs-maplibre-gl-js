<template>
  <mgl-map 
    mapStyle="https://api.maptiler.com/maps/streets/style.json?key=YOUR_MAPTILER_API_KEY_HERE"
    :zoom=14
    :center="[16.62662018, 49.2125578]"
  >
    <mgl-navigation-control position="top-left"/>
  </mgl-map>
</template>

<script>
import { MglMap, MglNavigationControl } from 'vue-maplibre-gl'

export default {
  name: 'App',
  components: {
    MglMap,
    MglNavigationControl
  }
}
</script>

<style lang="scss">
@import "~vue-maplibre-gl/src/css/maplibre.scss";

body {
  margin: 0;
  font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', 'Roboto', 'Oxygen',
    'Ubuntu', 'Cantarell', 'Fira Sans', 'Droid Sans', 'Helvetica Neue',
    sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}

code {
  font-family: source-code-pro, Menlo, Monaco, Consolas, 'Courier New', monospace;
}

#app {
  width: 100%;
  height: 100vh;
}
</style>
