<template>
  <div class="min-h-screen bg-gray-900 text-white font-sans">
    <Navigation />
    
    <div class="container mx-auto flex flex-col lg:flex-row pt-16">

      <Sidebar />
      

      <MainContent />
    </div>
  </div>
</template>

<script>
import Navigation from './components/Navigation.vue'
import Sidebar from './components/sidebar.vue'
import MainContent from './components/MainContent.vue'

export default {
  name: 'App',
  components: {
    Navigation,
    Sidebar,
    MainContent
  }
}
</script>