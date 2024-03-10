<template>
    <div class="w-[87%] bg-dark-darker overflow-scroll">


        <div class="flex justify-between px-10 py-4 bg-black sticky top-0 z-20">
            <div class="flex gap-x-5 items-center">
                <div class="space-x-2">
                    <button class="p-[0.20rem] bg-dark-light rounded-full">
                        <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5"
                            stroke="currentColor" class="w-6 h-6">
                            <path stroke-linecap="round" stroke-linejoin="round" d="M15.75 19.5L8.25 12l7.5-7.5" />
                        </svg>
                    </button>
                    <button class="p-[0.20rem] bg-dark-light rounded-full">
                        <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5"
                            stroke="currentColor" class="w-6 h-6">
                            <path stroke-linecap="round" stroke-linejoin="round" d="M8.25 4.5l7.5 7.5-7.5 7.5" />
                        </svg>
                    </button>
                </div>

                <div class="relative">
                    <input class="w-72 pl-10 pr-5 outline-none rounded-full h-10 text-black" type="text"
                        placeholder="¿Qué quieres escuchar?">
                    <div class="absolute top-2 left-3 text-black">
                        <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5"
                            stroke="currentColor" class="w-6 h-6">
                            <path stroke-linecap="round" stroke-linejoin="round"
                                d="M21 21l-5.197-5.197m0 0A7.5 7.5 0 105.196 5.196a7.5 7.5 0 0010.607 10.607z" />
                        </svg>
                    </div>
                </div>

            </div>

            <div class="flex gap-x-2">

                <button class="button-bordered">
                    Mejora tu cuenta
                </button>

                <button
                    class="h-8 flex items-center gap-x-1 pr-3 pl-[0.18rem] rounded-full text-sm font-semibold bg-dark hover:bg-neutral-900">
                    <div class="w-7 h-7 rounded-full overflow-hidden"><img src="/images/avatar.jpeg" alt=""></div>
                    <div>Jairo</div>
                    <div>
                        <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5"
                            stroke="currentColor" class="w-4 h-4">
                            <path stroke-linecap="round" stroke-linejoin="round" d="M19.5 8.25l-7.5 7.5-7.5-7.5" />
                        </svg>
                    </div>

                </button>

            </div>
        </div>



        <div class="px-10 pt-8 pb-28">

            <div class="flex gap-x-1">
                <div class="px-3 py-1 bg-light-primary text-black rounded-full">
                    Todo
                </div>

                <div class="px-3 py-1 bg-dark-light rounded-full">
                    Artista
                </div>

                <div class="px-3 py-1 bg-dark-light rounded-full">
                    Género
                </div>

                <div class="px-3 py-1 bg-dark-light rounded-full">
                    Álbumes
                </div>
            </div>

            <div class="flex flex-col lg:flex-row gap-x-5 gap-y-5 mt-5">
                <div class="w-full lg:w-2/5 ">
                    <h2 class="text-light-primary text-2xl font-bold">
                        Resultado principal
                    </h2>

                    <div class="mt-5 p-4 space-y-5 bg-dark-lighter rounded">
                        <div>
                            <img class="w-28 rounded rounded-full" src="/images/sacoto.jpeg" alt="">
                        </div>
                        <div>
                            <h2 class="text-light-primary text-3xl font-bold">Sergio Sacoto</h2>
                        </div>
                        <div class="flex">
                            <div class="px-3 py-1 font-semibold bg-dark-light rounded-full">
                                Artista
                            </div>
                        </div>
                    </div>
                </div>

                <div class="w-full lg:w-3/5">
                    <h2 class="text-light-primary text-2xl font-bold">
                        Canciones
                    </h2>

                    <div class="mt-5">
                        <div class="group p-2 flex justify-between items-center hover:bg-dark-light rounded">
                            <div class="flex gap-x-4">
                                <div class="relative">
                                    <img class="w-12 group-hover:brightness-50" src="/images/sacoto.jpeg" alt="">
                                    <svg class="absolute hidden group-hover:block top-[30%] left-[30%] w-6 h-6" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor">
                                        <path stroke-linecap="round" stroke-linejoin="round" d="M5.25 5.653c0-.856.917-1.398 1.667-.986l11.54 6.348a1.125 1.125 0 010 1.971l-11.54 6.347a1.125 1.125 0 01-1.667-.985V5.653z" />
                                    </svg>
                                </div>
                                <div>
                                    <h3>Al Borde (en vivo)</h3>
                                    <div class="text-sm"><a href="#" class="hover:underline">Sergio Sacoto</a></div>
                                </div>
                            </div>

                            <div class="flex gap-x-4">
                                <div class="px-5">
                                    <Like
                                        :like="true"
                                    >
                                    </Like>
                                </div>
                                <div class="text-light-secondary">
                                    4:39
                                </div>
                                <div>
                                    <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="w-6 h-6">
                                        <path stroke-linecap="round" stroke-linejoin="round" d="M6.75 12a.75.75 0 11-1.5 0 .75.75 0 011.5 0zM12.75 12a.75.75 0 11-1.5 0 .75.75 0 011.5 0zM18.75 12a.75.75 0 11-1.5 0 .75.75 0 011.5 0z" />
                                    </svg>
                                </div>
                            </div>
                        </div>

                        <div class="group p-2 flex justify-between items-center hover:bg-dark-light rounded">
                            <div class="flex gap-x-4">
                                <div class="relative">
                                    <img class="w-12 group-hover:brightness-50" src="/images/sacoto.jpeg" alt="">
                                    <svg class="absolute hidden group-hover:block top-[30%] left-[30%] w-6 h-6" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor">
                                        <path stroke-linecap="round" stroke-linejoin="round" d="M5.25 5.653c0-.856.917-1.398 1.667-.986l11.54 6.348a1.125 1.125 0 010 1.971l-11.54 6.347a1.125 1.125 0 01-1.667-.985V5.653z" />
                                    </svg>
                                </div>
                                <div>
                                    <h3>Al Borde (en vivo)</h3>
                                    <div class="text-sm"><a href="#" class="hover:underline">Sergio Sacoto</a></div>
                                </div>
                            </div>

                            <div class="flex gap-x-4">
                                <div class="px-5">
                                    <Like
                                        :like="true"
                                    >
                                    </Like>
                                </div>
                                <div class="text-light-secondary">
                                    4:39
                                </div>
                                <div>
                                    <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="w-6 h-6">
                                        <path stroke-linecap="round" stroke-linejoin="round" d="M6.75 12a.75.75 0 11-1.5 0 .75.75 0 011.5 0zM12.75 12a.75.75 0 11-1.5 0 .75.75 0 011.5 0zM18.75 12a.75.75 0 11-1.5 0 .75.75 0 011.5 0z" />
                                    </svg>
                                </div>
                            </div>
                        </div>

                        <div class="group p-2 flex justify-between items-center hover:bg-dark-light rounded">
                            <div class="flex gap-x-4">
                                <div class="relative">
                                    <img class="w-12 group-hover:brightness-50" src="/images/sacoto.jpeg" alt="">
                                    <svg class="absolute hidden group-hover:block top-[30%] left-[30%] w-6 h-6" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor">
                                        <path stroke-linecap="round" stroke-linejoin="round" d="M5.25 5.653c0-.856.917-1.398 1.667-.986l11.54 6.348a1.125 1.125 0 010 1.971l-11.54 6.347a1.125 1.125 0 01-1.667-.985V5.653z" />
                                    </svg>
                                </div>
                                <div>
                                    <h3>Al Borde (en vivo)</h3>
                                    <div class="text-sm"><a href="#" class="hover:underline">Sergio Sacoto</a></div>
                                </div>
                            </div>

                            <div class="flex gap-x-4">
                                <div class="px-5">
                                    <Like
                                        :like="true"
                                    >
                                    </Like>
                                </div>
                                <div class="text-light-secondary">
                                    4:39
                                </div>
                                <div>
                                    <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="w-6 h-6">
                                        <path stroke-linecap="round" stroke-linejoin="round" d="M6.75 12a.75.75 0 11-1.5 0 .75.75 0 011.5 0zM12.75 12a.75.75 0 11-1.5 0 .75.75 0 011.5 0zM18.75 12a.75.75 0 11-1.5 0 .75.75 0 011.5 0z" />
                                    </svg>
                                </div>
                            </div>
                        </div>

                        <div class="group p-2 flex justify-between items-center hover:bg-dark-light rounded">
                            <div class="flex gap-x-4">
                                <div class="relative">
                                    <img class="w-12 group-hover:brightness-50" src="/images/sacoto.jpeg" alt="">
                                    <svg class="absolute hidden group-hover:block top-[30%] left-[30%] w-6 h-6" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor">
                                        <path stroke-linecap="round" stroke-linejoin="round" d="M5.25 5.653c0-.856.917-1.398 1.667-.986l11.54 6.348a1.125 1.125 0 010 1.971l-11.54 6.347a1.125 1.125 0 01-1.667-.985V5.653z" />
                                    </svg>
                                </div>
                                <div>
                                    <h3>Al Borde (en vivo)</h3>
                                    <div class="text-sm"><a href="#" class="hover:underline">Sergio Sacoto</a></div>
                                </div>
                            </div>

                            <div class="flex gap-x-4">
                                <div class="px-5">
                                    <Like
                                        :like="true"
                                    >
                                    </Like>
                                </div>
                                <div class="text-light-secondary">
                                    4:39
                                </div>
                                <div>
                                    <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="w-6 h-6">
                                        <path stroke-linecap="round" stroke-linejoin="round" d="M6.75 12a.75.75 0 11-1.5 0 .75.75 0 011.5 0zM12.75 12a.75.75 0 11-1.5 0 .75.75 0 011.5 0zM18.75 12a.75.75 0 11-1.5 0 .75.75 0 011.5 0z" />
                                    </svg>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>


        </div>


    </div>
</template>

<script setup>
import Like from '../components/Like.vue';
</script>

