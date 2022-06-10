<template>
  <header class="w-10/12 mt-5 mx-auto">
    <div class="flex justify-between">
      <a href="/"><img class="w-3/12 h-auto " src="~/assets/Logo.png"></a>
      <div class="flex justify-end gap-4">
        <img class="w-1/12 h-auto" src="~assets/Heart.svg">
        <img class="w-1/12 h-auto cast" src="~assets/cast_google.svg">
        <img
          class="w-1/12 h-auto"
          src="~assets/download_rouge.svg"
          @onClick="promptInstall"
        >
      </div>
    </div>
    <div class="container mt-5">
      <p>Hi, <span class="font-bold">Emmanuelle !</span></p>
    </div>
  </header>
</template>
<script>
import { BeforeInstallPromptEvent } from 'vue-pwa-install'

export default {
  name: 'HeaderComponent',
  deferredPrompt: BeforeInstallPromptEvent,
  promptInstall () {
    this.deferredPrompt.prompt()
  }
}

</script>
<style>
#__layout{
  min-height: 100vh;
}
</style>
