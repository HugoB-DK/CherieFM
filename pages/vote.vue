<template>
  <div class="page-globale">
    <HeaderComponent />
    <Navbar />

    <div class="max-w-screen-xl mx-4 lg:mx-auto">
      <h1 class="text-xl my-2">
        Votes du jour
      </h1>
      <p class="mb-6">
        Vote pour la musique qui te fera <span class="text-red-700">vibrer</span> dans les prochaines minutes
      </p>
      <div class="flex w-100">
        <img src="~/assets/playlist2.jpeg" alt="" class="lg:w-28 w-14 rounded-l-lg">
        <div class="bg-gray-600 flex-auto rounded-r-lg flex flex-col justify-center pl-4 sm:pl-4">
          <h2 class="text-white uppercase">
            Le club chérie
          </h2>
          <span class="text-white font-light">POP</span>
        </div>
      </div>
      <h3 class="uppercase text-red-700 mt-12 mb-4">
        Sélectionnez une chanson
      </h3>
      <div class="grid grid-rows-2 gap-4">
        <div class="grid grid-cols-2 gap-2">
          <label class="">
            <input id="1" type="radio" name="music" class="absolute">
            <div>
              <img src="~/assets/sia.jpg" alt="" class="rounded-3xl border-4 border-lime-600 opacity-25 shadow-lg">
            </div>
          </label>
          <label class="">
            <input id="2" type="radio" name="music" class="absolute">
            <div>
              <img src="~/assets/clara_luciani.jpg" alt="" class="rounded-3xl border-4 border-lime-600 opacity-25 shadow-lg">
            </div>
          </label>
        </div>
        <div class="grid grid-cols-2 gap-2">
          <label class="">
            <input id="2" type="radio" name="music" class="absolute">
            <div>
              <img src="~/assets/ed-sheeran.webp" alt="" class="rounded-3xl border-4 border-lime-600 opacity-25 shadow-lg">
            </div>
          </label>
          <label class="">
            <input id="2" type="radio" name="music" class="absolute">
            <div>
              <img src="~/assets/eddy.jpeg" alt="" class="rounded-3xl border-4 border-lime-600 opacity-25 shadow-lg">
            </div>
          </label>
        </div>
        <div class="my-8 text-center">
          <button class="button-color text-white px-6 py-2 rounded-xl ">
            Je valide mon vote
          </button>
        </div>
      </div>
    </div>
    <FooterComponent />
  </div>
</template>

<script>
import Navbar from '~/components/Navbar.vue'
import HeaderComponent from '~/components/HeaderComponent.vue'
import FooterComponent from '~/components/FooterComponent.vue'

export default {
  name: 'VotePage',
  components: { HeaderComponent, Navbar, FooterComponent }
}

</script>

<style>
.page-globale{
  min-height: 100vh;
}
.button-color{
  background-color: #437F97;
}
.text-shadow{
  text-shadow: 0px 3px 6px #00000029;
}
input[type="radio"]{
  opacity: 0.1;
  z-index: 999;
  height: 0;
  width: 0;
}
input[type="checkbox"]:checked ~ img::after{
  opacity: 1;
}

input[type=radio] + div img {
  cursor: pointer;
}

input[type=radio]:checked + div img {
  outline: 2px solid #2EB636;
  opacity: 1;
}
</style>
