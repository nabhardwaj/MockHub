<template>
<GoogleMap api-key="AIzaSyAPo6QzCTVYg5OYvfhrsS16O4kreWpmiEw" style="width: 100%; height:100%" :center="center" :zoom="15">
    <Marker :options="{ position: center }" />
  </GoogleMap>
</template>
<script>
    import { defineComponent } from "vue";
import { GoogleMap, Marker } from "vue3-google-map";

export default defineComponent({
  components: { GoogleMap, Marker },
  setup() {
    const center = { lat: 26.9124336, lng: 75.7872709 };

    return { center };
  },
});
</script>