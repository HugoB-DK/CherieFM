<template>
  <div class="page-globale">
    <HeaderComponent />
    <Navbar />
    <div class="max-w-screen-xl mx-4 lg:mx-auto">
      <h1>Podcasts</h1>
      <p>Meilleurs podcasts de la semaines</p>

      <h2>Catégories</h2>
      <div class="grid grid-cols-2 gap-1">
        <div class="card pastel-green h-16 text-white rounded-lg relative overflow-hidden flex items-center mb-6">
          <h3 class="ml-4">
            Actualités
          </h3>
          <div class="card-info bg-white absolute text-xxs w-14 -right-0.5 p-2 -bottom-2 text-pastel-green rounded-lg">
            Les dernières actus
          </div>
        </div>

        <div class="card pastel-yellow h-16 text-white rounded-lg relative overflow-hidden flex items-center mb-6">
          <h3 class="ml-4">
            Ecoutez l'histoire
          </h3>
          <div class="card-info bg-white absolute text-xxs w-14 -right-0.5 p-2 -bottom-2 text-pastel-yellow rounded-lg">
            18e 19e 20e
          </div>
        </div>

        <div class="card pastel-gray h-16 text-white rounded-lg relative overflow-hidden flex items-center mb-6">
          <h3 class="ml-4">
            Enfants
          </h3>
          <div class="card-info bg-white absolute text-xxs w-14 -right-0.5 p-2 -bottom-2 text-pastel-gray rounded-lg">
            0 à 3 ans que faire ?
          </div>
        </div>

        <div class="card pastel-black h-16 text-white rounded-lg relative overflow-hidden flex items-center mb-6">
          <h3 class="ml-4">
            Lifestyle et méditation
          </h3>
          <div class="card-info bg-white absolute text-xxs w-14 -right-0.5 p-2 -bottom-2 text-pastel-black rounded-lg">
            inspirez puis expirez
          </div>
        </div>

        <div class="card pastel-yellow h-16 text-white rounded-lg relative overflow-hidden flex items-center mb-6">
          <h3 class="ml-4">
            Actualités
          </h3>
          <div class="card-info bg-white absolute text-xxs w-14 -right-0.5 p-2 -bottom-2 text-pastel-yellow rounded-lg">
            Les dernières actus
          </div>
        </div>

        <div class="card pastel-blue h-16 text-white rounded-lg relative overflow-hidden flex items-center mb-6">
          <h3 class="ml-4">
            Ecoutez l'histoire
          </h3>
          <div class="card-info bg-white absolute text-xxs w-14 -right-0.5 p-2 -bottom-2 text-pastel-blue rounded-lg">
            Les dernières actus
          </div>
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

.pastel-green{
    background-color: #7DAA92;
    border: 2px solid #7DAA92
}
.text-pastel-green{
    color: #7DAA92;
}

.pastel-yellow{
    background-color: #E8C547;
    border: 2px solid #E8C547;
}
.text-pastel-yellow{
    color: #E8C547;
}

.pastel-gray{
    background-color: #30323D;
    border: 2px solid #30323D;
}
.text-pastel-gray{
    color: #30323D;
}

.pastel-black{
    background-color: #002626;
    border: 2px solid #002626;
}
.text-pastel-black{
    color: #002626;
}
.pastel-blue{
    background-color: #003049;
    border: 2px solid #003049;
}
.text-pastel-blue{
    color: #003049;
}
.text-xxs{
    font-size: 8px;
}
.card-info{
    transform: rotate(15deg);
}
</style>
