<template>
  <div class="bg-slate-950 flex mt-20 relative bg-gradient-to-br from-yellow-600/20 via-transparent">
    <div class="home flex container m-auto h-auto sm:h-[calc(95vh-8vh)]">
      <!-- Grid -->
      <div class="grid m-auto grid-cols-1 lg:grid-cols-2">
        
        <!-- Coluna de texto -->
        <div class="flex flex-col mx-10 justify-center h-full ps-0 pt-10 sm:pt-5 sm:ps-10 md:ps-14 space-y-6">
          <!-- Título -->
          <h1 class="text-5xl font-extrabold text-slate-100 md:text-6xl lg:text-7xl dark:text-white">
            Bar<span class="text-yellow-500">Barone</span>
          </h1>

          <!-- Parágrafo -->
          <p class="text-lg text-slate-200 dark:text-neutral-400">
            Lorem ipsum dolor sit amet, consectetur adipisicing elit. Dolorum libero cupiditate eligendi. Distinctio dicta doloribus unde quibusdamia.
          </p>

          <!-- Botões -->
          <div class="flex flex-row justify-center sm:justify-start">
            <a class="py-3 px-6 inline-flex justify-center items-center gap-x-2 text-sm font-medium rounded-lg border-slate-200 bg-white text-slate-800 shadow-sm hover:bg-green-400 focus:outline-none focus:bg-slate-200"
              href="#">
              WhatsApp
              <i class="fab text-xl fa-whatsapp"></i>
            </a>
            <a class="py-3 px-6 ms-5 inline-flex justify-center items-center gap-x-2 text-sm font-medium rounded-lg border border-transparent bg-yellow-500 text-white hover:bg-yellow-600 focus:outline-none focus:bg-yellow-600"
              href="#">
              Get started
              <i class="fas fa-chevron-right"></i>
            </a>
          </div>
        </div>

        <!-- Coluna de imagem -->
        <div class="relative flex items-center justify-center">
          <!-- Imagem responsiva -->
          <div class="img-container w-8/12 h-[400px] sm:h-[450px] md:h-[50vh] lg:h-[60vh] my-12 overflow-hidden rounded-2xl shadow-lg">
            <img class="w-full h-full object-cover" 
              src="/fachada.jpeg" 
              alt="Hero Image"
            />
          </div>
        </div>

      </div>
    </div>
  </div>
</template>

<style scoped>
.img-container {
  box-shadow: 10px 10px 0px rgb(184, 155, 7);
}
</style>
