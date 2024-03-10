<template>
    <div class="w-[87%] bg-dark-darker overflow-scroll">


        <div class="flex justify-between px-10 py-4 bg-black sticky top-0 z-20">
        <div class="space-x-2">

            <button class="p-[0.20rem] bg-dark-light rounded-full">
            <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="w-6 h-6">
                <path stroke-linecap="round" stroke-linejoin="round" d="M15.75 19.5L8.25 12l7.5-7.5" />
            </svg>
            </button>
            <button class="p-[0.20rem] bg-dark-light rounded-full">
            <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="w-6 h-6">
                <path stroke-linecap="round" stroke-linejoin="round" d="M8.25 4.5l7.5 7.5-7.5 7.5" />
            </svg>
            </button>

        </div>

        <div class="flex gap-x-2">

            <button class="button-bordered">
            Mejora tu cuenta
            </button>

            <button class="h-8 flex items-center gap-x-1 pr-3 pl-[0.18rem] rounded-full text-sm font-semibold bg-dark hover:bg-neutral-900" >
            <div class="w-7 h-7 rounded-full overflow-hidden"><img src="/images/avatar.jpeg" alt=""></div>
            <div>Jairo</div>
            <div>
                <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="w-4 h-4">
                <path stroke-linecap="round" stroke-linejoin="round" d="M19.5 8.25l-7.5 7.5-7.5-7.5" />
                </svg>
            </div>

            </button>

        </div>
        </div>



        <div class="px-10 pt-14 pb-28">
        <div class="flex justify-between">
            <h2>
            <a href="#" class="text-light-primary text-2xl font-bold hover:underline">
                Escuchados recientemente
            </a>
            </h2>
            <button class="font-bold text-light-secondary text-sm hover:underline">Mostrar todos</button>
        </div>

        <div class="mt-8 grid grid-rows-1 grid-cols-3 lg:grid-cols-4 xl:grid-cols-5 2xl:grid-cols-6 3xl:grid-cols-8 gap-x-5">

            <Tile
            title="Sergio Sacoto"
            sub-title="Artista"
            image="/images/sacoto.jpeg"
            ></Tile>

            <Tile
            title="Enanitos Verdes"
            sub-title="Artista"
            image="/images/enanitos.jpeg"
            ></Tile>

            <Tile
            title="00s RockAnthems"
            sub-title="These songs rocked the 00s. Cover: Green Day"
            image="/images/rock.jpeg"
            shape="square"
            ></Tile>

            <Tile
            title="Enanitos Verdes"
            sub-title="Artista"
            image="/images/enanitos.jpeg"
            ></Tile>

            <Tile
            title="Enanitos Verdes"
            sub-title="Artista"
            image="/images/enanitos.jpeg"
            ></Tile>

        </div>


        </div>
    </div>
</template>

<script setup>
import Tile from '../components/Tile.vue';
</script>
