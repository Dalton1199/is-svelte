<script>
	import Icon from '@iconify/svelte';
    import Header from '../components/Header.svelte'

	import cisco from '../public/Cisco-Fuente.png'
	import java from '../public/java.png'
	import sql from '../public/sql.png'
	import raspberry from '../public/raspberry.png'
	import ubuntu from '../public/ubuntu.png'
	import shap from '../public/num_shap.png'

	import ingRoberto from '../public/profiles/roberto.png'
	import ingNazarena from '../public/profiles/nazarena.png'
	import ingGerardo from '../public/profiles/gerardo.png'
	import ingVargas from '../public/profiles/vargas.png'
	import ingBrand from '../public/profiles/brand.png'
	import ingJuan from '../public/profiles/alvarenga.png'
	import ingChacon from '../public/profiles/chacon.png'
	import ingLara from '../public/profiles/lara.png'
	import ingBorjas from '../public/profiles/borjas.png'
	import ingCubilla from '../public/profiles/cubilla.png'
	import ingLiliana from '../public/profiles/liliana.png'
	import ingDavid from '../public/profiles/david.png'
	import ingJulio from '../public/profiles/julio.png'
	import ingAlba from '../public/profiles/alba.png'

	import code from '../public/icons/browser.png'
	import cpu from '../public/icons/cpu.png'
	import data from '../public/icons/data-storage.png'
	import network from '../public/icons/network.png'
	import networkOne from '../public/icons/network-1.png'
	import chart from '../public/icons/pie-chart.png'
	import component from '../public/icons/video-card.png'

	import { onMount } from 'svelte'
  	import anime from "animejs";
	import { inview } from 'svelte-inview';
	
	function handleView() {
		anime({targets: '#countOne',value: [0, 514],round: 1,easing: 'easeInOutExpo', duration: 1500});
		anime({targets: '#countTwo',value: [0, 15],round: 1,easing: 'easeInOutExpo', duration: 1500});
		anime({targets: '#countThree',value: [0, 56],round: 1,easing: 'easeInOutExpo', duration: 1500});
		anime({targets: '#countFour',value: [0, 215],round: 1,easing: 'easeInOutExpo', duration: 1500});
	}

	onMount(async () => {
    });



</script>


<Header/>

<div class="">
	<section>
		<div class="relative bg-gradient-to-r rounded-lg from-blue-700 to-blue-500 mx-auto max-w-screen-xl px-8 py-16 md:px-36 md:pb-24 md:pt-20 lg:pt-0">
			<img class="absolute left-0 top-0 w-full h-full flex items-stretch px-8 py-4 opacity-30" src={shap} alt="">
			<div class="hidden flex-row justify-between pt-12 pb-1 mb-10 border-b border-white lg:flex">
				<div class="flex items-center">
					<img class="w-32" src={cisco} alt="">
				</div>
				<div class="flex items-center">
					<img class="w-24" src={java} alt="">
				</div>
				<div class="flex items-center">
					<img class="w-44" src={sql} alt="">
				</div>
				<div class="flex items-center">
					<img class="w-48" src={raspberry} alt="">
				</div>
				<div class="flex items-center">
					<img class="w-36" src={ubuntu} alt="">
				</div>
			</div>
			<div class="grid lg:grid-cols-2 md:grid-cols-1">
				<div class="flex items-center">
					<h2 class="text-white text-bold text-4xl md:mb-3">Creamos, Transformamos y Simplificamos</h2>
				</div>
				<div>
					<p class="text-lg text-white">Nuestras ??reas de ense??anza corresponden a Circuitos y Electr??nica, Desarrollo de Software, Base de Datos y Redes de Datos, permitiendo al estudiante al culminar su carrera poder desempe??arse en cualquiera de estas ??reas y as?? mismo poder realizar una perfecta integraci??n de todas ellas, posibilitando el desarrollo de proyecto de alta calidad y cumpliendo con todos los requisitos que el cliente desea.</p>
				</div>
			</div>
			<div class="grid xs:grid-cols-1 sm:grid-cols-2 lg:grid-cols-4 pt-16"  
				use:inview
				on:enter={handleView}
			>
				<div class="text-white font-medium text-center pb-8 md:pb-0">
					<input class="w-full text-center inline-block p-0 bg-transparent text-5xl" id="countOne">
					<p class="text-2xl mt-3">Estudiantes</p>
				</div>
				<div class="text-white font-medium text-center pb-8 md:pb-0">
					<input class="w-full text-center inline-block p-0 bg-transparent text-5xl" id="countTwo">
					<p class="text-2xl mt-3">Catedr??ticos</p>
				</div>
				<div class="text-white font-medium text-center pb-8 md:pb-0">
					<input class="w-full text-center inline-block p-0 bg-transparent text-5xl" id="countThree">
					<p class="text-2xl mt-3">Clases</p>
				</div>
				<div class="text-white font-medium text-center pb-8 md:pb-0">
					<input class="w-full text-center inline-block p-0 bg-transparent text-5xl" id="countFour">
					<p class="text-2xl mt-3">UV</p>
				</div>
			</div>
		</div>
	</section>


	<!-- Conocimientos -->
	<section class="py-4">
		<div class="mx-auto max-w-screen-xl px-4 py-16 sm:px-6 lg:px-8">
		  <div class="mx-auto max-w-2xl text-center">
			<h4 class="font-bold text-lg text-gray-600">Conoce</h4>
			<h3 class="text-blue-700 mb-6 md:text-3xl text-2xl md:leading-normal leading-normal font-semibold">??reas de Conocimiento</h3>
	  
			<p class="mt-4 text-slate-500 max-w-xl mx-auto">Es una rama de la Ingenier??a que implica la planificaci??n, dise??o, desarrollo, implementaci??n y mantenimiento de 
				los sistemas de informaci??n, que usan las diferentes empresas u organizaciones para procesar datos y producir informaci??n, que ayude 
				en la toma de decisiones.</p>
		  </div>
	  
		  <div class="mt-8 grid xs:grid-cols-1 sm:grid-cols-2 gap-8 md:grid-cols-3 lg:grid-cols-3">
			<div class="block p-8 rounded-md shadow-md">
				<h2 class="mt-4 text-xl font-medium text-gray-800 mb-5 text-center">Bases de Datos</h2>
				<div class="mb-5 p-3 rounded-md">
					<img src={cpu} alt="" class="w-1/3 m-auto">
				</div>
			  	<p class="text-md text-gray-500">Ser capaz de gestionar sistemas de almacenamiento distribuido. Crear sistemas de reportes de forma que sea posible ver los datos de forma sencilla.</p>
			</div>

			<div class="block p-8 rounded-md shadow-md">
				<h2 class="mt-4 text-xl font-medium text-gray-800 mb-5 text-center">Redes de Datos</h2>
				<div class="mb-5 p-3 rounded-md">
					<img src={network} alt="" class="w-1/3 m-auto">
				</div>
			  	<p class="text-md text-gray-500">Son redes de comunicaci??n en las que se han dise??ado para transmitir datos y es un m??todo eficaz de compartir la informaci??n a los usuarios aumentando la productividad, evitar la duplicaci??n del equipo y de los recursos.</p>
			</div>

			<div class="block p-8 rounded-md shadow-md">
				<h2 class="mt-4 text-xl font-medium text-gray-800 mb-5 text-center">Programaci??n</h2>
				<div class="mb-5 p-3 rounded-md">
					<img src={code} alt="" class="w-1/3 m-auto">
				</div>
			  	<p class="text-md text-gray-500">Ser capaz de gestionar sistemas de almacenamiento distribuido. Crear sistemas de reportes de forma que sea posible ver los datos de forma sencilla.</p>
			</div>

			<div class="block p-8 rounded-md shadow-md">
				<h2 class="mt-4 text-xl font-medium text-gray-800 mb-5 text-center">Electr??nica</h2>
				<div class="mb-5 p-3 rounded-md">
					<img src={component} alt="" class="w-1/3 m-auto">
				</div>
			  	<p class="text-md text-gray-500">Es una disciplina considerada como rama de la f??sica aplicada, y una especializaci??n de la ingenier??a. Trata con los circuitos electr??nicos que forman parte de los dispositivos que utilizamos a diario.</p>
			</div>

			<div class="block p-8 rounded-md shadow-md">
				<h2 class="mt-4 text-xl font-medium text-gray-800 mb-5 text-center">Seguridad Inform??tica</h2>
				<div class="mb-5 p-3 rounded-md">
					<img src={networkOne} alt="" class="w-1/3 m-auto">
				</div>
			  	<p class="text-md text-gray-500">Ser capaz de gestionar sistemas de almacenamiento distribuido. Crear sistemas de reportes de forma que sea posible ver los datos de forma sencilla.</p>
			</div>

			<div class="block p-8 rounded-md shadow-md">
				<h2 class="mt-4 text-xl font-medium text-gray-800 mb-5 text-center">Inteligencia Artifical</h2>
				<div class="mb-5 p-3 rounded-md">
					<img src={data} alt="" class="w-1/3 m-auto">
				</div>
			  	<p class="text-md text-gray-500">Ser capaz de gestionar sistemas de almacenamiento distribuido. Crear sistemas de reportes de forma que sea posible ver los datos de forma sencilla.</p>
			</div>
	  
		  </div>
		</div>
	  </section>	
	  
	  <section class="py-4">
		<div class="mx-auto max-w-screen-xl px-4 sm:px-6 lg:px-8">
			<div class="container md:mt-24 mt-16">
                <div class="mx-auto max-w-2xl text-center mb-16">
					<h4 class="font-bold text-lg text-gray-600">Conoce</h4>
					<h3 class="text-blue-700 mb-6 md:text-3xl text-2xl md:leading-normal leading-normal font-semibold">A Nuestros Catedr??ticos</h3>
			  
					<p class="mt-4 text-slate-400 max-w-xl mx-auto">A continuaci??n, te invitamos a conocer a algunos de los miembros de nuestro equipo de docentes en Ingenier??a en Sistemas, quienes est??n compuesto por expertos en la materia, profesionales apasionados cuya motivaci??n y dedicaci??n a su trabajo es vital para el ??xito de los estudiantes de la carrera.</p>
				</div>

                <div class="flex items-center flex-wrap justify-center mt-8">
                    <div class="h-full flex items-stretch sm:w-full md:w-1/2 lg:w-1/3 px-8 py-4">
                        <div class="w-full text-center team p-6 rounded-md shadow-md dark:shadow-gray-800 dark:border-gray-700 bg-white dark:bg-slate-900 relative">
                            <div class="absolute inset-0 bg-slate-300/10 dark:bg-slate-300/30 rounded-md -mt-[10px] -ml-[10px] h-[98%] w-[98%] z-[-1]"></div>
                            <img src={ingRoberto} class="h-24 w-24 m-auto rounded-full shadow-md dark:shadow-gray-800 object-cover" alt="">

                            <div class="content mt-4">
                                <span class="text-lg font-medium block mb-2">Ing. Roberto Hern??ndez</span>
                                <span class="text-slate-400 block mb-2">Programaci??n</span>
                                <a href="mailto:roberto.hernandez@unah.edu.hn" class="pt-4 text-slate-500 flex flex-row items-center justify-center">
									<Icon icon="ph:envelope-simple-light" class="text-xl mr-2" />
									<span>roberto.hernandez@unah.edu.hn</span></a>
                            </div>
                        </div>
                    </div>
                    
                    <div class="h-full flex items-stretch sm:w-full md:w-1/2 lg:w-1/3 px-8 py-4">
                        <div class="w-full text-center team p-6 rounded-md shadow-md dark:shadow-gray-800 dark:border-gray-700 bg-white dark:bg-slate-900 relative">
                            <div class="absolute inset-0 bg-emerald-300/10 dark:bg-emerald-300/30 rounded-md -mt-[10px] -ml-[10px] h-[98%] w-[98%] z-[-1]"></div>
                            <img src={ingNazarena} class="h-24 w-24 m-auto rounded-full shadow-md dark:shadow-gray-800 object-cover" alt="">

                            <div class="content mt-4">
                                <span class="text-lg font-medium block mb-2">Ing. Nazarena Idi??quez</span>
                                <span class="text-slate-400 block mb-2">Administraci??n</span>
                                <a href="mailto:nazarena.idiaquez@unah.edu.hn" class="pt-4 text-slate-500 flex flex-row items-center justify-center"><Icon icon="ph:envelope-simple-light" class="text-xl mr-2" /> <span>nazarena.idiaquez@unah.edu.hn</span></a>
							</div>
                        </div>
                    </div>
                    
                    <div class="h-full flex items-stretch sm:w-full md:w-1/2 lg:w-1/3 px-8 py-4">
                        <div class="w-full text-center team p-6 rounded-md shadow-md dark:shadow-gray-800 dark:border-gray-700 bg-white dark:bg-slate-900 relative">
                            <div class="absolute inset-0 bg-red-300/10 dark:bg-red-300/30 rounded-md -mt-[10px] -ml-[10px] h-[98%] w-[98%] z-[-1]"></div>
                            <img src={ingGerardo} class="h-24 w-24 m-auto rounded-full shadow-md dark:shadow-gray-800 object-cover" alt="">

                            <div class="content mt-4">
                                <span class="text-lg font-medium block mb-2">Ing. Gerardo Portillo</span>
                                <span class="text-slate-400 block mb-2">Programaci??n</span>

                                <a href="mailto:gerardo.portillo@unah.edu.hn" class="pt-4 text-slate-500 flex flex-row items-center justify-center"><Icon icon="ph:envelope-simple-light" class="text-xl mr-2" /> <span>gerardo.portillo@unah.edu.hn</span></a>
                            </div>
                        </div>
                    </div>

					<div class="h-full flex items-stretch sm:w-full md:w-1/2 lg:w-1/3 px-8 py-4">
                        <div class="w-full text-center team p-6 rounded-md shadow-md dark:shadow-gray-800 dark:border-gray-700 bg-white dark:bg-slate-900 relative">
                            <div class="absolute inset-0 bg-blue-300/10 dark:bg-blue-300/30 rounded-md -mt-[10px] -ml-[10px] h-[98%] w-[98%] z-[-1]"></div>
                            <img src={ingVargas} class="h-24 w-24 m-auto rounded-full shadow-md dark:shadow-gray-800 object-cover" alt="">

                            <div class="content mt-4">
                                <span class="text-lg font-medium block mb-2">Ing. Jorge Vargas</span>
                                <span class="text-slate-400 block mb-2">Electr??nica</span>

                                <a href="mailto:jorge.vargas@unah.edu.hn" class="pt-4 text-slate-500 flex flex-row items-center justify-center"><Icon icon="ph:envelope-simple-light" class="text-xl mr-2" /> <span>jorge.vargas@unah.edu.hn</span></a>
                            </div>
                        </div>
                    </div>

					<div class="h-full flex items-stretch sm:w-full md:w-1/2 lg:w-1/3 px-8 py-4">
                        <div class="w-full text-center team p-6 rounded-md shadow-md dark:shadow-gray-800 dark:border-gray-700 bg-white dark:bg-slate-900 relative">
                            <div class="absolute inset-0 bg-slate-300/10 dark:bg-slate-300/30 rounded-md -mt-[10px] -ml-[10px] h-[98%] w-[98%] z-[-1]"></div>
                            <img src={ingBrand} class="h-24 w-24 m-auto rounded-full shadow-md dark:shadow-gray-800 object-cover" alt="">

                            <div class="content mt-4">
                                <span class="text-lg font-medium block mb-2">Ing. Guillermo Brand</span>
                                <span class="text-slate-400 block mb-2">Seguridad Inform??tica</span>
                                <a href="mailto:guillermo.brand@unah.edu.hn" class="pt-4 text-slate-500 flex flex-row items-center justify-center"><Icon icon="ph:envelope-simple-light" class="text-xl mr-2" /> <span>guillermo.brand@unah.edu.hn</span></a>
                            </div>
                        </div>
                    </div>
                    
                    <div class="h-full flex items-stretch sm:w-full md:w-1/2 lg:w-1/3 px-8 py-4">
                        <div class="w-full text-center team p-6 rounded-md shadow-md dark:shadow-gray-800 dark:border-gray-700 bg-white dark:bg-slate-900 relative">
                            <div class="absolute inset-0 bg-emerald-300/10 dark:bg-emerald-300/30 rounded-md -mt-[10px] -ml-[10px] h-[98%] w-[98%] z-[-1]"></div>
                            <img src={ingChacon} class="h-24 w-24 m-auto rounded-full shadow-md dark:shadow-gray-800 object-cover" alt="">

                            <div class="content mt-4">
                                <span class="text-lg font-medium block mb-2">Ing. Mar??a Chac??n</span>
                                <span class="text-slate-400 block mb-2">Administraci??n</span>
                                <a href="mailto:maria.chacon@unah.edu.hn" class="pt-4 text-slate-500 flex flex-row items-center justify-center"><Icon icon="ph:envelope-simple-light" class="text-xl mr-2" /> <span>maria.chacon@unah.edu.hn</span></a>
							</div>
                        </div>
                    </div>
                    
                    <div class="h-full flex items-stretch sm:w-full md:w-1/2 lg:w-1/3 px-8 py-4">
                        <div class="w-full text-center team p-6 rounded-md shadow-md dark:shadow-gray-800 dark:border-gray-700 bg-white dark:bg-slate-900 relative">
                            <div class="absolute inset-0 bg-red-300/10 dark:bg-red-300/30 rounded-md -mt-[10px] -ml-[10px] h-[98%] w-[98%] z-[-1]"></div>
                            <img src={ingJuan} class="h-24 w-24 m-auto rounded-full shadow-md dark:shadow-gray-800 object-cover" alt="">

                            <div class="content mt-4">
                                <span class="text-lg font-medium block mb-2">Ing. Juan Alvarenga</span>
                                <span class="text-slate-400 block mb-2">Programaci??n Web</span>

                                <a href="mailto:jealvarengar@unah.edu.hn" class="pt-4 text-slate-500 flex flex-row items-center justify-center"><Icon icon="ph:envelope-simple-light" class="text-xl mr-2" /> <span>jealvarengar@unah.edu.hn</span></a>
                            </div>
                        </div>
                    </div>

					<div class="h-full flex items-stretch sm:w-full md:w-1/2 lg:w-1/3 px-8 py-4">
                        <div class="w-full text-center team p-6 rounded-md shadow-md dark:shadow-gray-800 dark:border-gray-700 bg-white dark:bg-slate-900 relative">
                            <div class="absolute inset-0 bg-blue-300/10 dark:bg-blue-300/30 rounded-md -mt-[10px] -ml-[10px] h-[98%] w-[98%] z-[-1]"></div>
                            <img src={ingLara} class="h-24 w-24 m-auto rounded-full shadow-md dark:shadow-gray-800 object-cover" alt="">

                            <div class="content mt-4">
                                <span class="text-lg font-medium block mb-2">Ing. Lara Norori</span>
                                <span class="text-slate-400 block mb-2">Administraci??n</span>

                                <a href="mailto:lara.norori@unah.edu.hn" class="pt-4 text-slate-500 flex flex-row items-center justify-center"><Icon icon="ph:envelope-simple-light" class="text-xl mr-2" /> <span>lara.norori@unah.edu.hn</span></a>
                            </div>
                        </div>
                    </div>

					<div class="h-full flex items-stretch sm:w-full md:w-1/2 lg:w-1/3 px-8 py-4">
                        <div class="w-full text-center team p-6 rounded-md shadow-md dark:shadow-gray-800 dark:border-gray-700 bg-white dark:bg-slate-900 relative">
                            <div class="absolute inset-0 bg-slate-300/10 dark:bg-slate-300/30 rounded-md -mt-[10px] -ml-[10px] h-[98%] w-[98%] z-[-1]"></div>
                            <img src={ingBorjas} class="h-24 w-24 m-auto rounded-full shadow-md dark:shadow-gray-800 object-cover" alt="">

                            <div class="content mt-4">
                                <span class="text-lg font-medium block mb-2">Ing. Guillermo Borjas</span>
                                <span class="text-slate-400 block mb-2">Bases de Datos</span>
                                <a href="mailto:guillermo.borjas@unah.edu.hn" class="pt-4 text-slate-500 flex flex-row items-center justify-center"><Icon icon="ph:envelope-simple-light" class="text-xl mr-2" /> <span>guillermo.borjas@unah.edu.hn</span></a>
                            </div>
                        </div>
                    </div>
                    
                    <div class="h-full flex items-stretch sm:w-full md:w-1/2 lg:w-1/3 px-8 py-4">
                        <div class="w-full text-center team p-6 rounded-md shadow-md dark:shadow-gray-800 dark:border-gray-700 bg-white dark:bg-slate-900 relative">
                            <div class="absolute inset-0 bg-emerald-300/10 dark:bg-emerald-300/30 rounded-md -mt-[10px] -ml-[10px] h-[98%] w-[98%] z-[-1]"></div>
                            <img src={ingCubilla} class="h-24 w-24 m-auto rounded-full shadow-md dark:shadow-gray-800 object-cover" alt="">

                            <div class="content mt-4">
                                <span class="text-lg font-medium block mb-2">Ing. Norman Cubilla</span>
                                <span class="text-slate-400 block mb-2">Arquitectura</span>
                                <a href="mailto:norman.cubilla@unah.edu.hn" class="pt-4 text-slate-500 flex flex-row items-center justify-center"><Icon icon="ph:envelope-simple-light" class="text-xl mr-2" /> <span>norman.cubilla@unah.edu.hn</span></a>
							</div>
                        </div>
                    </div>
                    
                    <div class="h-full flex items-stretch sm:w-full md:w-1/2 lg:w-1/3 px-8 py-4">
                        <div class="w-full text-center team p-6 rounded-md shadow-md dark:shadow-gray-800 dark:border-gray-700 bg-white dark:bg-slate-900 relative">
                            <div class="absolute inset-0 bg-red-300/10 dark:bg-red-300/30 rounded-md -mt-[10px] -ml-[10px] h-[98%] w-[98%] z-[-1]"></div>
                            <img src={ingLiliana} class="h-24 w-24 m-auto rounded-full shadow-md dark:shadow-gray-800 object-cover" alt="">

                            <div class="content mt-4">
                                <span class="text-lg font-medium block mb-2">Ing. Liliana Ir??as</span>
                                <span class="text-slate-400 block mb-2">Administraci??n</span>

                                <a href="mailto:liliana.irias@unah.edu.hn" class="pt-4 text-slate-500 flex flex-row items-center justify-center"><Icon icon="ph:envelope-simple-light" class="text-xl mr-2" /> <span>liliana.irias@unah.edu.hn</span></a>
                            </div>
                        </div>
                    </div>

					<div class="h-full flex items-stretch sm:w-full md:w-1/2 lg:w-1/3 px-8 py-4">
                        <div class="w-full text-center team p-6 rounded-md shadow-md dark:shadow-gray-800 dark:border-gray-700 bg-white dark:bg-slate-900 relative">
                            <div class="absolute inset-0 bg-blue-300/10 dark:bg-blue-300/30 rounded-md -mt-[10px] -ml-[10px] h-[98%] w-[98%] z-[-1]"></div>
                            <img src={ingDavid} class="h-24 w-24 m-auto rounded-full shadow-md dark:shadow-gray-800 object-cover" alt="">

                            <div class="content mt-4">
                                <span class="text-lg font-medium block mb-2">Ing. David Rivera</span>
                                <span class="text-slate-400 block mb-2">Redes de Datos</span>
                                <a href="mailto:roberto.hernandez@unah.edu.hn" class="pt-4 text-slate-500 flex flex-row items-center justify-center"><Icon icon="ph:envelope-simple-light" class="text-xl mr-2" /> <span>roberto.hernandez@unah.edu.hn</span></a>
                            </div>
                        </div>
                    </div>

					<div class="h-full flex items-stretch sm:w-full md:w-1/2 lg:w-1/3 px-8 py-4">
                        <div class="w-full text-center team p-6 rounded-md shadow-md dark:shadow-gray-800 dark:border-gray-700 bg-white dark:bg-slate-900 relative">
                            <div class="absolute inset-0 bg-emerald-300/10 dark:bg-emerald-300/30 rounded-md -mt-[10px] -ml-[10px] h-[98%] w-[98%] z-[-1]"></div>
                            <img src={ingJulio} class="h-24 w-24 m-auto rounded-full shadow-md dark:shadow-gray-800 object-cover" alt="">

                            <div class="content mt-4">
                                <span class="text-lg font-medium block mb-2">Ing. Julio Hern??ndez</span>
                                <span class="text-slate-400 block mb-2">Seminario</span>
                                <a href="mailto:jchernandez@unah.edu.hn" class="pt-4 text-slate-500 flex flex-row items-center justify-center"><Icon icon="ph:envelope-simple-light" class="text-xl mr-2" /> <span>jchernandez@unah.edu.hn</span></a>
                            </div>
                        </div>
                    </div>

					<div class="h-full flex items-stretch sm:w-full md:w-1/2 lg:w-1/3 px-8 py-4">
                        <div class="w-full text-center team p-6 rounded-md shadow-md dark:shadow-gray-800 dark:border-gray-700 bg-white dark:bg-slate-900 relative">
                            <div class="absolute inset-0 bg-red-300/10 dark:bg-red-300/30 rounded-md -mt-[10px] -ml-[10px] h-[98%] w-[98%] z-[-1]"></div>
                            <img src={ingAlba} class="h-24 w-24 m-auto rounded-full shadow-md dark:shadow-gray-800 object-cover" alt="">

                            <div class="content mt-4">
                                <span class="text-lg font-medium block mb-2">Lic. Alba Arias</span>
                                <span class="text-slate-400 block mb-2">Contabilidad</span>
                                <a href="mailto:alba.arias@unah.edu.hn" class="pt-4 text-slate-500 flex flex-row items-center justify-center"><Icon icon="ph:envelope-simple-light" class="text-xl mr-2" /> <span>alba.arias@unah.edu.hn</span></a>
                            </div>
                        </div>
                    </div>

    
                </div>
            </div><!--end container-->
		</div>
	  </section>

	  <footer class="absolute mb-0 w-full mt-16 bg-gradient-to-r from-blue-700 to-blue-500 px-8 py-4">
		<div class="mx-auto max-w-screen-xl">
			<h2 class="text-center text-white text-lg">Ingenier??a en Sistemas - UNAH-VS</h2>
		</div>

	</footer>
</div>