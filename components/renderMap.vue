<template>
  <v-layout class="mapper">
    <no-ssr>
      <l-map
        :zoom="10"
        :center="[7.1907, 125.4553]">
        <l-tile-layer url="https://api.mapbox.com/v4/mapbox.streets/{z}/{x}/{y}.png?access_token=pk.eyJ1IjoicGVkcm9qdWFucCIsImEiOiJjam91bHk1cTUxOW40M3htbHgzaHJsdXNpIn0.JRRzAl1-biNVdrYCEedzvg"/>
        <l-marker :lat-lng="[47.413220, -1.219482]"/>
      </l-map>
    </no-ssr>
  </v-layout>
</template>

<style scoped>
.mapper {
  height: 500px;
}
</style>
