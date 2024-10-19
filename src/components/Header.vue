<script setup>
import { ref, onMounted, onBeforeUnmount } from 'vue';

const modoEscuro = ref(false);
const scrolled = ref(false);  // Indica se a página foi rolada

const updateModoEscuro = () => {
    modoEscuro.value = document.documentElement.classList.contains('dark');
};

onMounted(() => {
    updateModoEscuro();

    // Observer para escutar as mudanças de classe
    const observer = new MutationObserver(() => {
        updateModoEscuro();
    });

    observer.observe(document.documentElement, {
        attributes: true,
        attributeFilter: ['class']
    });

    // Função que vai monitorar o scroll
    const handleScroll = () => {
        if (window.scrollY > 50) { // Se rolou mais de 50px
            scrolled.value = true;
        } else {
            scrolled.value = false;
        }
    };

    // Adiciona o evento de scroll
    window.addEventListener('scroll', handleScroll);

    // Remove o evento de scroll quando o componente for destruído
    onBeforeUnmount(() => {
        window.removeEventListener('scroll', handleScroll);
    });
});

const alteraModo = () => {
    const html = document.documentElement;
    const isDark = html.classList.toggle('dark');
    localStorage.setItem('darkMode', isDark);
};

const savedMode = localStorage.getItem('darkMode');
if (savedMode === 'true') {
    document.documentElement.classList.add('dark');
}
</script>

<template>
    <div :class="['header fixed top-0 w-full transition-all duration-300 py-1 bg-slate-950 shadow-2xl ', { 'h-14 bg-opacity-40 shadow-none': scrolled, 'h-20 bg-opacity-100': !scrolled }]" :style="{ zIndex: 50 }">
        <div class="container flex items-center justify-between mx-auto px-4 h-full">
            <!-- Logo -->
            <div class="flex-shrink-0 flex items-center justify-center">
                <img v-if="modoEscuro" class="h-10 transition-all duration-300" :class="{ 'h-12': scrolled, 'h-16': !scrolled }" src="/icone.png" alt="Ícone" />
                <img v-else class="h-10 transition-all duration-300" :class="{ 'h-12': scrolled, 'h-16': !scrolled }" src="/icone.png" alt="Ícone" />
            </div>

            <!-- Navegação (oculta em dispositivos móveis) -->
            <nav class="hidden md:flex items-center space-x-6 text-white">
                <a class="text-base sm:text-lg font-normal hover:text-dark-grey-900 transition duration-200" href="#">Início</a>
                <a class="text-base sm:text-lg font-normal hover:text-dark-grey-900 transition duration-200" href="#">Parceiros</a>
                <a class="text-base sm:text-lg font-normal hover:text-dark-grey-900 transition duration-200" href="#">Produtos</a>
                <a @click="alteraModo" class="text-base sm:text-lg font-normal hover:text-dark-grey-900 transition duration-200" href="#">
                    <i :class="modoEscuro ? 'fa-regular fa-moon' : 'fa-regular fa-sun'"></i>
                </a>
            </nav>

            <!-- Botão "Fazer Orçamento" -->
            <div class="flex-shrink-0">
                <button :class="['flex items-center font-bold px-4 py-2 rounded-xl bg-yellow-500 text-slate-100 hover:bg-yellow-600 hover:text-slate-200 transition duration-300', { 'text-sm': scrolled, 'text-lg': !scrolled }]">
                    Fazer Orçamento
                </button>
            </div>
        </div>
    </div>
</template>

<style scoped>
</style>
