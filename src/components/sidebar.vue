<template>
  <aside class="w-full lg:w-80 bg-gray-800 p-6 lg:min-h-screen">
    <!-- Foto de Perfil -->
    <div class="text-center mb-8">
      <img src="/public/image/foto-facebook.jpg" alt="foto-perfil" 
          class="w-32 h-32 rounded-full mx-auto border-4 border-blue-500 shadow-lg object-cover">
    </div>

    <div class="text-center mb-8">
      <h1 class="text-2xl font-bold text-white">Ivanildo Santos</h1>
      <p class="text-blue-400 font-semibold mt-2">Desenvolvedor Web</p>
    </div>

    <hr class="border-gray-600 mb-8">

    <div class="mb-8">
      <h2 class="text-lg font-semibold mb-4 text-white">Contato</h2>
      <div class="space-y-3">
        <div class="flex items-center text-gray-300">
          <i class="fas fa-envelope mr-3 text-blue-400"></i>
          <span>ivandearaujodev@gmail.com</span>
        </div>
        <div class="flex items-center text-gray-300">
          <i class="fas fa-phone mr-3 text-blue-400"></i>
          <span>(86) 995880501</span>
        </div>
        <div class="flex items-center text-gray-300">
          <i class="fas fa-map-marker-alt mr-3 text-blue-400"></i>
          <span>Parnaíba, PI</span>
        </div>
      </div>
    </div>

    <div class="mb-8">
      <h2 class="text-lg font-semibold mb-4 text-white">Redes Sociais</h2>
      <div class="flex flex-col space-y-3">

      <a href="#" class="flex items-center text-gray-300 hover:text-blue-400 transition">
      <span>LinkedIn</span>
        <i class="fab fa-linkedin text-blue-400 ml-2"></i>
        </a>

        <a href="https://github.com/IvandearaujoBs" class="flex items-center text-gray-300 hover:text-blue-400 transition" target="_blank" rel="noopener">
          <span>Github</span>
          <i class="fab fa-github  text-blue-400 ml-2"></i>
        </a>

        <a href="#" class="flex items-center text-gray-300 hover:text-blue-400 transition">
          <span>Instagram</span>
          <i class="fab fa-instagram text-blue-400 ml-2"></i>
        </a>

      </div>
    </div>

    <div>
      <h2 class="text-lg font-semibold  text-white mb-4">Tecnologias</h2>
      <div class="flex flex-wrap gap-2">
        <span class="bg-gray-700 px-3 py-1 rounded-full text-sm  hover:text-blue-400">JavaScript</span>
        <span class="bg-gray-700 px-3 py-1 rounded-full text-sm  hover:text-blue-400">TypeScript</span>
        <span class="bg-gray-700 px-3 py-1 rounded-full text-sm  hover:text-blue-400">Python</span>
        <span class="bg-gray-700 px-3 py-1 rounded-full text-sm  hover:text-blue-400">Vue.js</span>
        <span class="bg-gray-700 px-3 py-1 rounded-full text-sm  hover:text-blue-400">React</span>
        <span class="bg-gray-700 px-3 py-1 rounded-full text-sm  hover:text-blue-400">Node.js</span>
        <span class="bg-gray-700 px-3 py-1 rounded-full text-sm  hover:text-blue-400">Tailwind</span>
        <span class="bg-gray-700 px-3 py-1 rounded-full text-sm  hover:text-blue-400">MySQL</span>
        <span class="bg-gray-700 px-3 py-1 rounded-full text-sm  hover:text-blue-400">SQLite</span>
      </div>
    </div>
  </aside>
</template>

<script>
export default {
  name: 'Sidebar'
}
</script>