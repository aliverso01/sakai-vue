<template>
  <div style="height: 600px; width: 100%;">
    <l-map ref="map" v-model:zoom="zoom" :center="[LMarkers[0].lat, LMarkers[0].lng]">
      <l-tile-layer
        url="https://{s}.tile.openstreetmap.org/{z}/{x}/{y}.png"
        layer-type="base"
        name="OpenStreetMap"
      ></l-tile-layer>
      <l-marker
        v-for="(marker, index) in LMarkers"
        :key="index"
        :lat-lng="[marker.lat, marker.lng]"
      ></l-marker>
    </l-map>
  </div>
</template>

<script>
import "leaflet/dist/leaflet.css";
import { LMap, LTileLayer, LMarker } from "@vue-leaflet/vue-leaflet";

export default {
  components: {
    LMap,
    LTileLayer,
    LMarker,
  },
  data() {
    return {
      zoom: 13,
      LMarkers: [
        { lat: -5.79448, lng: -35.211 }, // Centro
        { lat: -5.79974, lng: -35.23101 }, // Ponta Negra
        { lat: -5.81809, lng: -35.21386 }, // Lagoa Nova
        { lat: -5.77004, lng: -35.24565 }, // Redinha
        { lat: -5.74161, lng: -35.21253 }, // Genipabu
        { lat: -5.82232, lng: -35.20507 }, // Cidade Satélite
        { lat: -5.86458, lng: -35.18764 }, // Parnamirim
        { lat: -5.83036, lng: -35.20092 }, // Alecrim
        { lat: -5.76361, lng: -35.21944 }, // Tirol
        { lat: -5.84584, lng: -35.21172 }, // Capim Macio
      ],
    };
  },
};
</script>

<style></style>
