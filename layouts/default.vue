<template>
    <div class="relative bg-">

        <Head>
            <link rel="stylesheet" href="https://fonts.googleapis.com/icon?family=Material+Icons">
        </Head>
        <header>

            <nav class="navbar fixed top-0 w-full bg-white  dark:bg-gray-900">
                <div class="max-w-screen-xl flex flex-wrap items-center  justify-between mx-auto p-4">
                    <a href="#" class="flex items-center">
                        <!-- <img src="https://flowbite.com/docs/images/logo.svg" class="h-8 mr-3" alt="Flowbite Logo" /> -->
                        <span class="self-center text-2xl font-semibold whitespace-nowrap dark:text-white">mahdi</span>
                    </a>
                    <button @click="openmenu" data-collapse-toggle="navbar-default" type="button"
                        class="inline-flex items-center p-2 w-10 h-10 justify-center text-sm text-gray-500 rounded-lg md:hidden hover:bg-gray-100 focus:outline-none focus:ring-2 focus:ring-gray-200 dark:text-gray-400 dark:hover:bg-gray-700 dark:focus:ring-gray-600"
                        aria-controls="navbar-default" aria-expanded="false">
                        <span class="sr-only">Open main menu</span>
                        <div :class="isActive ? 'block' : 'hidden'" class="self-center justify-self-center">

                            <i class="material-icons  mt-1  ">remove</i>
                        </div>
                        <svg :class="isActive ? 'hidden' : 'block'" class="w-5 h-5 " aria-hidden="true"
                            xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 17 14">
                            <path stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                                d="M1 1h15M1 7h15M1 13h15" />
                        </svg>

                    </button>
                    <div ref="navbar_default" :class="isActive ? 'block' : 'hidden'" class=" w-full md:block md:w-auto"
                        id="navbar-default">
                        <ul
                            class="font-medium flex flex-col p-4 md:p-0 mt-4  rounded-lg bg-gray-50 md:flex-row md:space-x-8 md:mt-0 md:border-0 md:bg-white dark:bg-gray-800 md:dark:bg-gray-900 dark:border-gray-700">
                            <li>
                                <a href="#"
                                    class="block py-2 pl-3 pr-4  text-gray-900  rounded hover:bg-slate-950  hover:text-white md:bg-transparent  md:p-0 dark:text-white md:text-black md:hover:bg-black md:hover:text-yellow-50 transition-all ease-linear duration-200 md:dark:text-blue-500"
                                    aria-current="page">Home</a>
                            </li>
                            <li>
                                <a href="#about"
                                    class="block py-2 pl-3 pr-4 text-gray-900    rounded hover:bg-slate-950 hover:text-white md:border-0 md:text-black md:hover:bg-black md:hover:text-yellow-50 transition-all ease-linear duration-200 md:p-0 dark:text-white md:dark:hover:text-blue-500 dark:hover:bg-gray-700 dark:hover:text-white md:dark:hover:bg-transparent">About</a>
                            </li>
                            <li>
                                <a href="#Skills"
                                    class="block py-2 pl-3 pr-4 text-gray-900   rounded hover:bg-slate-950 hover:text-white md:text-black md:hover:bg-black md:hover:text-yellow-50 transition-all ease-linear duration-200 md:p-0 dark:text-white md:dark:hover:text-blue-500 dark:hover:bg-gray-700 dark:hover:text-white md:dark:hover:bg-transparent">Skills</a>
                            </li>
                            <li>
                                <a href="#Services"
                                    class="block py-2 pl-3 pr-4 text-gray-900  rounded hover:bg-slate-950 hover:text-white md:text-black md:hover:bg-black md:hover:text-yellow-50 transition-all ease-linear duration-200 md:p-0 dark:text-white md:dark:hover:text-blue-500 dark:hover:bg-gray-700 dark:hover:text-white md:dark:hover:bg-transparent">Services</a>
                            </li>
                            <li>
                                <a href="#"
                                    class="block py-2 pl-3 pr-4 text-gray-900 rounded hover:bg-slate-950 hover:text-white md:text-black md:hover:bg-black md:hover:text-yellow-50 transition-all ease-linear duration-200 md:p-0 dark:text-white md:dark:hover:text-blue-500 dark:hover:bg-gray-700 dark:hover:text-white md:dark:hover:bg-transparent">Portfolio</a>
                            </li>
                            <li>
                                <a href="#"
                                    class="block py-2 pl-3 pr-4 text-gray-900 rounded hover:bg-slate-950 hover:text-white md:text-black md:hover:bg-black md:hover:text-yellow-50 transition-all ease-linear duration-100 md:p-0 dark:text-white md:dark:hover:text-blue-500 dark:hover:bg-gray-700 dark:hover:text-white md:dark:hover:bg-transparent">Contact</a>
                            </li>
                        </ul>
                    </div>
                </div>
            </nav>

        </header>
        <slot />
    </div>
</template>

<script setup>
import { ref } from 'vue'
const navbar_default = ref(null)
const isActive = ref(false)
function openmenu() {
    isActive.value = !isActive.value
    console.log(navbar_default.value.classList.value)
}
</script>

<style  scoped></style>