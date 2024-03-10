<template>
    <div class="w-[87%] bg-dark-darker overflow-scroll">


        <div class="flex justify-between px-10 py-4 bg-black sticky top-0 z-20">
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

        <div class="pt-5 pb-7 flex from-amber-800 to-amber-900 bg-gradient-to-b">
            <div class="w-1/4">
                <div class="w-52 h-52 mx-auto mt-4 overflow-hidden rounded-full">
                    <img class="w-full h-full object-cover" src="/images/enanitos.jpeg" >
                </div>
            </div>
            <div class="w-3/4 pt-24 space-y-7">
                <div class="text-7xl font-semibold">Los Enanitos Verdes</div>
                <div>
                    10.697.849 oyentes mensuales
                </div>
            </div>
        </div>

        <div class="from-amber-950 to-dark bg-gradient-to-b to-40%">
            <div class="px-7 py-5 flex items-center gap-x-7">
                <div>
                    <button>
                        <svg class="w-16 h-16 text-green-primary hover:scale-105 hover:text-green-secondary transition" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor">
                            <path stroke-linecap="round" stroke-linejoin="round" d="M21 12a9 9 0 11-18 0 9 9 0 0118 0z" />
                            <path stroke-linecap="round" stroke-linejoin="round" d="M15.91 11.672a.375.375 0 010 .656l-5.603 3.113a.375.375 0 01-.557-.328V8.887c0-.286.307-.466.557-.327l5.603 3.112z" />
                        </svg>
                    </button>
                </div>
                <div>
                    <button class="border px-4 py-1 font-semibold text-sm tracking-widest rounded uppercase">Siguiendo</button>
                </div>
                <div>
                    <svg class="w-10 h-10 text-light-secondary hover:text-light-primary" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor">
                        <path stroke-linecap="round" stroke-linejoin="round" d="M6.75 12a.75.75 0 11-1.5 0 .75.75 0 011.5 0zM12.75 12a.75.75 0 11-1.5 0 .75.75 0 011.5 0zM18.75 12a.75.75 0 11-1.5 0 .75.75 0 011.5 0z" />
                    </svg>
                </div>
            </div>

            <div class="px-7 pb-28">
                <h2 class="text-2xl font-semibold">Populares</h2>

                <div class="mt-3">
                    <Track
                        :track-number="1"
                        image="/images/soda.jpeg"
                        track-name="Al borde (en vivo)"
                        duration="4:58"
                        :like="true"
                    ></Track>
                    <Track
                        :track-number="2"
                        image="/images/sacoto.jpeg"
                        track-name="Lamento Boliviano"
                        duration="3:42"
                        :like="false"
                    ></Track>
                    <Track
                        :track-number="3"
                        image="/images/nickel.jpeg"
                        track-name="La Muralla Verde"
                        duration="2:41"
                        :like="true"
                    ></Track>
                    <Track
                        :track-number="4"
                        image="/images/soda.jpeg"
                        track-name="Tu carcel - En Vivo"
                        duration="4:02"
                        :like="false"
                    ></Track>
                    <Track
                        :track-number="5"
                        image="/images/nickel.jpeg"
                        track-name="Mariposas"
                        duration="3:41"
                        :like="true"
                    ></Track>
                </div>
                <div class="ml-5 mt-4">
                    <a href="#" class="text-light-secondary hover:text-light-primary font-semibold">See more</a>
                </div>
            </div>
        </div>

    </div>
</template>

<script setup>
import Track from '../components/Track.vue';
</script>
