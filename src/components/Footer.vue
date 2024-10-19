<script setup>
import { ref, onMounted } from 'vue';

const modoEscuro = ref(false);

const updateModoEscuro = () => {
	modoEscuro.value = document.documentElement.classList.contains('dark');
};

const anoAtual = new Date().getFullYear()

onMounted(() => {
	updateModoEscuro();

	const observer = new MutationObserver(() => {
		updateModoEscuro();
	});

	observer.observe(document.documentElement, {
		attributes: true,
		attributeFilter: ['class']
	});
});
</script>

<template>
	<footer class="px-4 divide-y bg-slate-950 text-slate-700 dark:text-slate-300">
		<div class="container flex flex-col justify-between py-10 mx-auto space-y-8 lg:flex-row lg:space-y-0">

			<img class="h-24 m-auto object-contain" src="/icone.png" alt="Ícone" />
			<div class="grid grid-cols-2 text-sm gap-x-3 gap-y-8 px-3 sm?px-0 lg:w-2/3 sm:grid-cols-4">
				<div class="space-y-3">
					<h3 class="text-slate-300 text-2xl">Opções</h3>
					<ul class="space-y-1 text-md">
						<li class="text-gray-200 hover:text-gray-400">
							<a href="#">Início</a>
						</li>
						<li class="text-gray-200 hover:text-gray-400">
							<a href="#">Profissionais</a>
						</li>
						<li class="text-gray-200 hover:text-gray-400">
							<a href="#">Produtos</a>
						</li>
					</ul>
				</div>
				<div class="space-y-3">
					<h3 class="text-slate-300 text-2xl">Em Marília/SP</h3>
					<ul class="space-y-1 text-md">
						<li class="text-gray-200 hover:text-gray-400">
							<a href="#">
								<i class="fas fa-location-dot"></i>
								Rua Ângelo Seleghini, 870</a>
						</li>
						<li class="text-gray-200 hover:text-gray-400">
							<a href="#">
								<i class="fab fa-whatsapp"></i>
								(14) 9 98808-9328
							</a>
						</li>
					</ul>
				</div>
				<div class="space-y-3">
					<div class="text-slate-300 text-2xl">Redes Sociais</div>
					<div class="flex justify-start space-x-3 text-gray-50 hover:text-gray-200">
						<a target="_blank" href="https://www.instagram.com/barba_rone?igsh=MWdzcnVmdzdxN2F1dQ=="
							title="instagram" class="flex items-center p-1">
							<i class="fa-brands fa-instagram text-4xl"></i>
						</a>
						<a target="_blank" href="#"
							title="linkedin" class="flex items-center p-1">
							<i class="fa-brands fa-google text-4xl"></i>
						</a>
					</div>
				</div>

				<div class="">
					<a href="http://gdmd.digital" target="_blank" class="flex justify-center lg:justify-start">
						<div class="flex items-center justify-center w-12 h-12">
							<img class="h-16" src="/icondark.png">
							<!-- v-if="modoEscuro"  <img v-else class="h-20" src="/icon.png"> -->
						</div>
						<span class="self-end ps-2 sm:ps-0 text-white text-xl font-semibold">Marketing
							Digital</span>
					</a>
				</div>
			</div>
		</div>
		<div class="py-6 text-sm text-center dark:text-slate-500">© {{ anoAtual }} Barbarone. Todos os direitos
			reservados.</div>
	</footer>
</template>
