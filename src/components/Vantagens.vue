<script setup>
import { ref } from 'vue'

const mostrarModal = ref(false)

// Função para fechar o modal
const fecharModal = () => {
  mostrarModal.value = false
}
</script>

<template>
    <div class="bg-slate-950 bg-gradient-to-bl from-yellow-600/20 via-transparent">
        <div class="max-w-5xl px-4 xl:px-0 py-10 lg:pt-20 lg:pb-20 mx-auto">
            <div class="max-w-5xl mb-10 lg:mb-14 flex flex-col lg:flex-row text-center lg:text-start items-center">
                <img class="h-26 order-1 lg:order-1" src="/icone.png" alt="Ícone" />
                <p class="mt-1 text-slate-300 px-3 order-2 lg:order-2">
                    This profound insight guides our comprehensive strategy — from meticulous research and strategic
                    planning to
                    the seamless execution of brand development and website or product deployment.
                </p>
            </div>
            <div class="grid px-4 grid-cols-1 lg:grid-cols-2 gap-10 lg:gap-16 lg:items-center">
                <div class="img-container rounded-xl">
                    <img class="img" src="/fachada.jpeg" alt="Features Image">
                </div>
                <div>

                    <div class="mb-4">
                        <h3 class="text-yellow-500 text-xs font-medium uppercase">
                            Steps
                        </h3>
                    </div>
                    <div class="flex gap-x-5 ms-1">
                        <div
                            class="relative last:after:hidden after:absolute after:top-8 after:bottom-0 after:start-4 after:w-px after:-translate-x-[0.5px] after:bg-neutral-800">
                            <div class="relative z-10 size-8 flex justify-center items-center">
                                <span
                                    class="flex shrink-0 justify-center items-center size-8 border border-neutral-800 text-yellow-500 font-semibold text-xs uppercase rounded-full">1</span>
                            </div>
                        </div>
                        <div class="grow pt-0.5 pb-8 sm:pb-12">
                            <p class="text-sm lg:text-base text-neutral-400">
                                <span class="text-white">Market Research and Analysis:</span>
                                Identify your target audience and understand their needs, preferences, and behaviors.
                            </p>
                        </div>
                    </div>
                    <div class="flex gap-x-5 ms-1">
                        <div
                            class="relative last:after:hidden after:absolute after:top-8 after:bottom-0 after:start-4 after:w-px after:-translate-x-[0.5px] after:bg-neutral-800">
                            <div class="relative z-10 size-8 flex justify-center items-center">
                                <span
                                    class="flex shrink-0 justify-center items-center size-8 border border-neutral-800 text-yellow-500 font-semibold text-xs uppercase rounded-full">2</span>
                            </div>
                        </div>
                        <div class="grow pt-0.5 pb-8 sm:pb-12">
                            <p class="text-sm lg:text-base text-neutral-400">
                                <span class="text-white">Product Development and Testing:</span>
                                Develop digital products or services that address the needs and preferences of your
                                target audience.
                            </p>
                        </div>
                    </div>
                    <div class="flex gap-x-5 ms-1">
                        <div
                            class="relative last:after:hidden after:absolute after:top-8 after:bottom-0 after:start-4 after:w-px after:-translate-x-[0.5px] after:bg-neutral-800">
                            <div class="relative z-10 size-8 flex justify-center items-center">
                                <span
                                    class="flex shrink-0 justify-center items-center size-8 border border-neutral-800 text-yellow-500 font-semibold text-xs uppercase rounded-full">3</span>
                            </div>
                        </div>
                        <div class="grow pt-0.5 pb-8 sm:pb-12">
                            <p class="text-sm md:text-base text-neutral-400">
                                <span class="text-white">Marketing and Promotion:</span>
                                Develop a comprehensive marketing strategy to promote your digital products or services.
                            </p>
                        </div>
                    </div>
                    <div class="flex gap-x-5 ms-1">
                        <div
                            class="relative last:after:hidden after:absolute after:top-8 after:bottom-0 after:start-4 after:w-px after:-translate-x-[0.5px] after:bg-neutral-800">
                            <div class="relative z-10 size-8 flex justify-center items-center">
                                <span
                                    class="flex shrink-0 justify-center items-center size-8 border border-neutral-800 text-yellow-500 font-semibold text-xs uppercase rounded-full">4</span>
                            </div>
                        </div>
                        <div class="grow pt-0.5 pb-8 sm:pb-12">
                            <p class="text-sm md:text-base text-neutral-400">
                                <span class="text-white">Launch and Optimization:</span>
                                Launch your digital products or services to the market, closely monitoring their
                                performance and user feedback.
                            </p>
                        </div>
                    </div>
                    <a class="group inline-flex items-center gap-x-2 py-2 px-3 text-white bg-yellow-500 hover:bg-yellow-600 duration-300 font-medium text-sm text-neutral-800 rounded-full focus:outline-none"
                        @click="mostrarModal = true" href="javascript:void(0)">
                        <i class="fas fa-phone"></i>
                        Agendar Horário
                    </a>

                    <div v-if="mostrarModal" @click.self="fecharModal"
                        class="fixed inset-0 z-50 bg-black bg-opacity-50 flex items-center justify-center">
                        <div class="relative bg-gray-900 p-4 rounded-lg">
                            <button @click="fecharModal"
                                class="absolute top-0 right-1 text-gray-200 hover:text-gray-300">
                                <i class="fas fa-times"></i> 
                            </button>
                            <img src="/qr.png" alt="Qr Code" class="rounded-lg">
                        </div>
                    </div>

                </div>
            </div>
        </div>
    </div>

</template>

<style scoped>
.img-container {
    height: 600px;
    width: 100%;
    max-width: 500px;
    box-shadow: 10px 10px 0px rgb(184, 155, 7);
    overflow: hidden;
    margin: 0 auto;
}

.img {
    width: 100%;
    height: 100%;
    object-fit: cover;
}

@media (max-width: 768px) {
    .img-container {
        height: 400px;
        max-width: 100%;
    }

    .cone {
        width: 30vw;
        top: 65%;
        right: 0;
    }
}
</style>
