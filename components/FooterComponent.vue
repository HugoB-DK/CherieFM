<template>
  <footer class="absolute bottom-0 footer">
    <audio controls>
      <source src="http://scdn.nrjaudio.fm/adwz2/fr/30201/mp3_128.mp3?origine=fluxradios" type="audio/mp3">
    </audio>
  </footer>
</template>
<script>
export default {
  name: 'FooterComponent'
}
</script>
<style>
.footer{
  width: 100%;
  height: 60px;
  background-color: #D4000D;
}
audio::-webkit-media-controls-panel {
  background-color: #D4000D;
}

audio::-webkit-media-controls-volume-slider {
  background-color: #D4000D;
}
audio::-webkit-media-controls-timeline-container{
  display: none !important;
}
audio::-webkit-media-controls-current-time-display{
  display: none !important;
}
audio::-webkit-media-controls-timeline{
  display: none !important;
}
audio::-webkit-media-controls-volume-slider-container{
  display: none !important;
}
audio::-webkit-media-controls-volume-slider{
  display: none !important;
}
</style>
