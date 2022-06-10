<template>
  <header class="w-10/12 mt-5 mx-auto">
    <div class="flex justify-between">
      <img class="w-3/12 h-auto " src="~/assets/Logo.png">
      <div class="flex justify-end gap-4">
        <img class="w-1/12 h-auto" src="~assets/Heart.svg">
        <img class="w-1/12 h-auto cast" src="~assets/cast_google.svg">
        <img class="w-1/12 h-auto" src="~assets/download_rouge.svg">
      </div>
    </div>
    <div class="container mt-2">
      <p>Hi, <span class="font-bold">Emmanuelle !</span></p>
    </div>
  </header>
</template>
<script>
export default {
  name: 'HeaderComponent'
}
</script>
<style>
#__layout{
  min-height: 100vh;
}
</style>
