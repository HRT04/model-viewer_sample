<!-- YourModelViewerComponent.vue -->

<template>
  <div>
    <model-viewer
      ar
      alt="Leoモデル"
      :src="modelSrc"
      :ios-src="iosModelSrc"
      style="width: 800px; height: 1000px"
      background-color="#70BCD1"
      shadow-intensity="0.7"
      camera-controls
      interaction-prompt="auto"
      auto-rotate
      magic-leap
    ></model-viewer>
  </div>
</template>

<script>
export default {
  data() {
    return {
      modelSrc: "./rocket.glb",
      iosModelSrc: "./rocket.usdz",
    };
  },
};
</script>

<style>
/* 必要に応じてスタイルを追加 */
</style>
