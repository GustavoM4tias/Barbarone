<script setup>
import { ref } from 'vue'

const mostrarModal = ref(false)

// Função para fechar o modal
const fecharModal = () => {
  mostrarModal.value = false
}
</script>

<template>
  <div class="content w-full bg-slate-950 bg-gradient-to-r from-yellow-600/20 via-transparent">
    <div class="max-w-6xl px-4 py-10 sm:px-6 lg:px-8 lg:py-14 mx-auto">
      <div class="max-w-3xl mb-10 lg:mb-14 text-center m-auto">
        <h2 class="text-white font-semibold text-4xl md:text-6xl md:leading-tight">Insta<span
            class="text-yellow-500">gram</span></h2>
        <p class="mt-1 text-neutral-400">@barbarone</p>
      </div>
      <div class="grid sm:grid-cols-12 gap-6 text-center">
        <div class="sm:self-end col-span-12 sm:col-span-7 md:col-span-8 lg:col-span-5 lg:col-start-3">

          <a class="group relative block rounded-xl overflow-hidden focus:outline-none" href="#">
            <div class="aspect-w-12 aspect-h-7 sm:aspect-none rounded-xl overflow-hidden">
              <img
                class="group-hover:scale-105 group-focus:scale-105 transition-transform duration-500 ease-in-out rounded-xl w-full object-cover"
                src="https://images.unsplash.com/photo-1606868306217-dbf5046868d2?ixlib=rb-4.0.3&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=560&q=80"
                alt="Masonry Cards Image">
            </div>
            <div class="absolute bottom-0 start-0 end-0 p-2 sm:p-5">
              <div
                class="text-sm font-semibold text-gray-800 rounded-lg bg-white p-2 md:text-xl dark:bg-neutral-800 dark:text-neutral-200">
                Nova Fachada
              </div>
            </div>
          </a>
        </div>
        <div class="sm:self-end col-span-12 sm:col-span-5 md:col-span-4 lg:col-span-3">
          <a class="group relative block rounded-xl overflow-hidden focus:outline-none" href="#">
            <div class="aspect-w-12 aspect-h-7 sm:aspect-none rounded-xl overflow-hidden">
              <img
                class="group-hover:scale-105 group-focus:scale-105 transition-transform duration-500 ease-in-out rounded-xl w-full object-cover"
                src="https://images.unsplash.com/photo-1605629921711-2f6b00c6bbf4?ixlib=rb-4.0.3&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=560&q=80"
                alt="Masonry Cards Image">
            </div>
            <div class="absolute bottom-0 start-0 end-0 p-2 sm:p-5">
              <div
                class="text-sm font-semibold text-gray-800 rounded-lg bg-white p-2 md:text-xl dark:bg-neutral-800 dark:text-neutral-200">
                Women in engineering
              </div>
            </div>
          </a>
        </div>
        <div class="col-span-12 md:col-span-4">
          <a class="group relative block rounded-xl overflow-hidden focus:outline-none" href="#">
            <div class="aspect-w-12 aspect-h-7 sm:aspect-none rounded-xl overflow-hidden">
              <img
                class="group-hover:scale-105 group-focus:scale-105 transition-transform duration-500 ease-in-out rounded-xl w-full object-cover"
                src="https://images.unsplash.com/photo-1606836576983-8b458e75221d?ixlib=rb-4.0.3&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=560&q=80"
                alt="Masonry Cards Image">
            </div>
            <div class="absolute bottom-0 start-0 end-0 p-2 sm:p-5">
              <div
                class="text-sm font-semibold text-gray-800 rounded-lg bg-white p-2 md:text-xl dark:bg-neutral-800 dark:text-neutral-200">
                Pride 2021
              </div>
            </div>
          </a>
        </div>
        <div class="col-span-12 sm:col-span-6 md:col-span-4">
          <a class="group relative block rounded-xl overflow-hidden focus:outline-none" href="#">
            <div class="aspect-w-12 aspect-h-7 sm:aspect-none rounded-xl overflow-hidden">
              <img
                class="group-hover:scale-105 group-focus:scale-105 transition-transform duration-500 ease-in-out rounded-xl w-full object-cover"
                src="https://images.unsplash.com/photo-1598929438701-ef29ab0bb61a?ixlib=rb-4.0.3&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=560&q=80"
                alt="Masonry Cards Image">
            </div>
            <div class="absolute bottom-0 start-0 end-0 p-2 sm:p-5">
              <div
                class="text-sm font-semibold text-gray-800 rounded-lg bg-white p-2 md:text-xl dark:bg-neutral-800 dark:text-neutral-200">
                Grande Inauguracao
              </div>
            </div>
          </a>
        </div>
        <div class="col-span-12 sm:col-span-6 md:col-span-4">
          <a class="group relative block rounded-xl overflow-hidden focus:outline-none" href="#">
            <div class="aspect-w-12 aspect-h-7 sm:aspect-none rounded-xl overflow-hidden">
              <img
                class="group-hover:scale-105 group-focus:scale-105 transition-transform duration-500 ease-in-out rounded-xl w-full object-cover"
                src="https://images.unsplash.com/photo-1467043153537-a4fba2cd39ef?ixlib=rb-4.0.3&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=560&q=80"
                alt="Masonry Cards Image">
            </div>
            <div class="absolute bottom-0 start-0 end-0 p-2 sm:p-5">
              <div
                class="text-sm font-semibold text-gray-800 rounded-lg bg-white p-2 md:text-xl dark:bg-neutral-800 dark:text-neutral-200">
                Empowered management
              </div>
            </div>
          </a>
        </div>
      </div>
      <div class="mais flex pt-10">
        <a class="group inline-flex lg:hidden m-auto items-center gap-x-2 py-2 px-3 text-white bg-yellow-500 hover:bg-yellow-600 duration-300 text-lg text-neutral-800 rounded-xl focus:outline-none"
          href="https://www.instagram.com/barba_rone?igsh=MWdzcnVmdzdxN2F1dQ==" target="_blank">
          <i class="fab fa-instagram text-2xl"></i>
          Ver Mais
        </a>
        <a class="group hidden lg:inline-flex m-auto items-center gap-x-2 py-2 px-3 text-white bg-yellow-500 hover:bg-yellow-600 duration-300 text-lg text-neutral-800 rounded-xl focus:outline-none"
          @click="mostrarModal = true" href="javascript:void(0)">
          <i class="fab fa-instagram text-2xl"></i>
          Ver Mais
        </a>
      </div>



      <div v-if="mostrarModal" @click.self="fecharModal"
        class="fixed inset-0 z-50 bg-black bg-opacity-50 flex items-center justify-center">
        <div class="relative bg-black p-4 rounded-lg">
          <button @click="fecharModal" class="absolute top-0 right-1 text-gray-200 hover:text-gray-300">
            <i class="fas fa-times"></i>
          </button>
          <img src="/insta-qr.jpeg" alt="Qr Code" class="rounded-lg">
        </div>
      </div>


    </div>
  </div>


</template>