<template>
  <v-layout class="mapper">
    <no-ssr>
      <l-map
        :zoom="10"
        :center="[7.1907, 125.4553]">
        <l-tile-layer url="http://{s}.tile.osm.org/{z}/{x}/{y}.png"/>
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
