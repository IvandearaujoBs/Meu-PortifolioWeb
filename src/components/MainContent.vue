<template>
  <main class="flex-1 p-6 lg:p-8">

    <section id="sobre" class="mb-12">
      <h2 class="text-3xl font-bold mb-6 text-white">Sobre Mim</h2>
      <div class="bg-gray-800 rounded-lg p-6 shadow-lg">
        <p class="text-gray-300 leading-relaxed">
          Sou estudante de Sistemas de Computação na Universidade Estadual do Piauí (UESPI) 
          e tenho grande interesse na área de tecnologia, em especial no desenvolvimento web. 
          Gosto de criar soluções práticas e criativas, sempre buscando melhorar minhas habilidades 
          e aprender novas ferramentas que possam agregar aos meus projetos. Meu objetivo é evoluir 
          como desenvolvedor e construir aplicações que unam funcionalidade e uma boa experiência 
          para o usuário.
        </p>
      </div>
    </section>

    <section id="projetos" class="mb-12">
      <h2 class="text-3xl font-bold mb-6 text-white">Projetos</h2>
      <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-6">
        <div v-for="project in projects" :key="project.id" 
            class="bg-gray-800 rounded-lg p-6 shadow-lg hover:shadow-xl transition">
          <h3 class="text-xl font-semibold mb-3 text-white">{{ project.title }}</h3>
          <p class="text-gray-300 mb-4">{{ project.description }}</p>
          <div class="flex flex-wrap gap-2 mb-4">
            <span v-for="tech in project.technologies" :key="tech" 
                  class="bg-blue-500 px-2 py-1 rounded text-xs">
              {{ tech }}
            </span>
          </div>
          <a :href="project.link" class="text-blue-400 hover:text-blue-300 transition">
            Ver Projeto →
          </a>
        </div>
      </div>
    </section>

    <section id="experiencia" class="mb-12">
      <h2 class="text-3xl font-bold mb-6 text-white">Experiência</h2>
      <div class="space-y-6">
        <div v-for="exp in experience" :key="exp.id" 
            class="bg-gray-800 rounded-lg p-6 shadow-lg">
          <h3 class="text-xl font-semibold text-white">{{ exp.position }}</h3>
          <p class="text-blue-400 mb-2">{{ exp.company }} • {{ exp.period }}</p>
          <p class="text-gray-300">{{ exp.description }}</p>
        </div>
      </div>
    </section>
  </main>
</template>

<script>
export default {
  name: 'MainContent',
  data() {
    return {
      projects: [
        {
          id: 1,
          title: "Store Confeitaria",
          description: "E-commerce de Confeitaria integração com WhatsApp",
          technologies: ["Vue.js", "Node.js", "Tailwind CSS", "MySQL"],
          link: "#"
        },
        {
          id: 2,
          title: "Quiz Master",
          description: "Gerador de Questões com IA para estudantes ou professores",
          technologies: ["Next.js", "SQLite", "Tailwind CSS", "Grok API", "Javascript"],
          link: "#"
        },
        {
          id: 3,
          title: "StreamHub",
          description: "Plataforma de Streaming & Discovery",
          technologies: ["JavaScript ES6", "HTML5", "CSS", "Node.js", "fetch API"],
          link: "#"
        },
        {
          id: 4,
          title: "Gerenciamento de Filas de Pronto-Socorro",
          description: "Sistema de Triagem e Gestão Hospitalar",
          technologies: ["Next.js", "Tailwind CSS", "LocalStorage", "Typescript", "SQLite"],
          link: "#"
        }
      ],
      experience: [
        {
          id: 1,
          position: "Desenvolvedor Front-end",
          company: "Tech Solutions",
          period: "2023 - Presente",
          description: "Desenvolvimento de interfaces modernas e responsivas usando Vue.js e React."
        },
        {
          id: 2,
          position: "Estagiário em Desenvolvimento",
          company: "StartUp Inovação",
          period: "2022 - 2023",
          description: "Suporte no desenvolvimento de aplicações web e mobile."
        }
      ]
    }
  }
}
</script>