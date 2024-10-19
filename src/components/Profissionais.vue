<template>

  <div class="container-fluid bg-slate-950 p-5">
    <div class="max-w-[65rem] px-4 py-10 sm:px-6 lg:px-8 lg:py-14 mx-auto">
      <!-- Title -->
      <div class="max-w-2xl mx-auto text-center mb-10 lg:mb-14">
        <h2 class="text-4xl font-bold md:text-5xl md:leading-tight text-white">Nosso Time</h2>
        <p class="mt-1 text-gray-600 dark:text-neutral-400">Stay in the know with insights from industry experts.</p>
      </div>
      <!-- End Title -->

      <!-- Grid -->
      <div class="grid grid-cols-1 lg:grid-cols-2 gap-16">

        <!-- Card -->
        <a class="group relative block rounded-xl overflow-hidden focus:outline-none" href="#">
          <div class="aspect-w-12 aspect-h-7 h-full sm:aspect-none rounded-xl overflow-hidden">
            <img
              class="group-hover:scale-105 group-focus:scale-105 transition-transform duration-500 ease-in-out rounded-xl w-full h-full object-cover"
              src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSbW4a14KeDXII8iKtIRuA4Ds-whyE2nYy47A&s"
              alt="Masonry Cards Image">
          </div>
          <div class="absolute top-0 start-0 end-0 p-2 sm:p-5">
            <p class="p-2 drop-shadow-lg font-semibold text-slate-50 rounded-lg text-3xl md:text-4xl">
              Gabriel Barone
            </p>
          </div>
          <div class="absolute bottom-0 start-0 end-0 p-2 sm:p-5">
            <button
              class="p-2 font-semibold text-slate-50 group-hover:text-yellow-400 duration-200 drop-shadow hover:drop-shadow- rounded-lg text-xl md:text-2xl">
              Agendar Horário
              <i class="fas fa-chevron-right"></i>
            </button>
          </div>
        </a>
        <!-- End Card -->

        <!-- Card -->
        <a class="group relative block rounded-xl overflow-hidden focus:outline-none" href="#">
          <div class="aspect-w-12 aspect-h-7 h-full sm:aspect-none rounded-xl overflow-hidden">
            <img
              class="group-hover:scale-105 group-focus:scale-105 transition-transform duration-500 ease-in-out rounded-xl w-full h-full object-cover"
              src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQAqWwV0SCMPulAJXrX2HbMUpGNRERbXwxRzA&s"
              alt="Masonry Cards Image">
          </div>
          <div class="absolute top-0 start-0 end-0 p-2 sm:p-5">
            <p class="p-2 drop-shadow-lg font-semibold text-slate-50 rounded-lg text-3xl md:text-4xl">
              Sthefanie (Calíquinha)
            </p>
          </div>
          <div class="absolute bottom-0 start-0 end-0 p-2 sm:p-5">
            <button
              class="p-2 font-semibold text-slate-50 group-hover:text-yellow-400 duration-200 drop-shadow hover:drop-shadow- rounded-lg text-xl md:text-2xl">
              Agendar Horário
              <i class="fas fa-chevron-right"></i>
            </button>
          </div>
        </a>
        <!-- End Card -->

      </div>
      <!-- End Grid -->
    </div>
  </div>

</template>