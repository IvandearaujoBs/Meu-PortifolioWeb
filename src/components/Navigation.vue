<template>
  <nav class="fixed top-0 left-0 right-0 bg-gray-800 shadow-lg z-50">
    <div class="container mx-auto px-6 py-4">
      <div class="flex justify-between items-center">
        <div class="text-xl font-bold text-blue-400">
          Ivanildo Santos
        </div>
        
        <div class="hidden md:flex space-x-8">
          <a href="#inicio" class="hover:text-blue-400 transition">Início</a>
          <a href="#sobre" class="hover:text-blue-400 transition">Sobre</a>
          <a href="#projetos" class="hover:text-blue-400 transition">Projetos</a>
          <a href="#habilidades" class="hover:text-blue-400 transition">Habilidades</a>
          <a href="#contato" class="hover:text-blue-400 transition">Contato</a>
        </div>

        <!-- Mobile Menu Button -->
        <button class="md:hidden text-white">
          <i class="fas fa-bars text-xl"></i>
        </button>
      </div>
    </div>
  </nav>
</template>

<script>
export default {
  name: 'Navigation'
}
</script>