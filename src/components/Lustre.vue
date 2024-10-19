<template>
    <!-- Cone decorativo posicionado entre as seções -->
    <div class="absolute top-[calc(104vh)] right-0 transform -translate-y-1/2 z-10 hidden lg:block duration-300">
      <img class="w-[10vw] sm:w-[15vw] md:w-[20vw]" 
        src="https://static.wixstatic.com/media/b617de_0ae28b6b734f45d294ce0b04333ea481~mv2.png/v1/fill/w_744,h_744,al_c,q_90,usm_0.66_1.00_0.01,enc_auto/Barbershop%20Lamp_H03_2k.png"
        alt="Cone Decorativo">
    </div>
  </template>
  
  
  <style scoped>
  .absolute {
    filter: drop-shadow(-50px 100px 150px rgba(255, 255, 0, .7)) brightness(90%);
  }

  .absolute:hover {
    filter: drop-shadow(-80px 150px 150px rgba(255, 255, 0, 1)) brightness(110%);
    
  }
  </style>
  