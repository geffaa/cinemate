<template>
    <div>
        <nav class="bg-gray-200 border-gray-200 dark:bg-gray-900">
        <div class="w-full flex flex-wrap items-center justify-between mx-auto p-4">
            <NuxtLink to="/" class="flex items-center space-x-3 rtl:space-x-reverse">
                <img src="/logo.png" class="h-8" alt="Cinemate Logo" />
                <span class="self-center text-2xl font-semibold whitespace-nowrap dark:text-white">CINEMATE</span>
            </NuxtLink>
            <button data-collapse-toggle="navbar-default" type="button" class="inline-flex items-center p-2 w-10 h-10 justify-center text-sm text-gray-500 rounded-lg md:hidden hover:bg-gray-100 focus:outline-none focus:ring-2 focus:ring-gray-200 dark:text-gray-400 dark:hover:bg-gray-700 dark:focus:ring-gray-600" aria-controls="navbar-default" aria-expanded="false">
                <span class="sr-only">Open main menu</span>
                <svg class="w-5 h-5" aria-hidden="true" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 17 14">
                    <path stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M1 1h15M1 7h15M1 13h15"/>
                </svg>
            </button>
            <div class="hidden w-full md:block md:w-auto" id="navbar-default">
            <ul class="font-medium flex flex-col p-4 md:p-0 mt-4 border border-gray-200 rounded-lg bg-gray-200 md:flex-row md:space-x-8 rtl:space-x-reverse md:mt-0 md:border-0 md:bg-gray-200 dark:bg-gray-800 md:dark:bg-gray-900 dark:border-gray-700">
                <li>
                <NuxtLink exact to="/" exact-active-class="text-blue-700" class="block py-2 px-3 md:p-0 rounded md:bg-transparent">Home</NuxtLink>
                </li>
                <li>
                <NuxtLink exact to="/search" exact-active-class="text-blue-700" class="block py-2 px-3 text-gray-900 rounded hover:bg-gray-100 md:hover:bg-transparent md:border-0 md:hover:text-blue-700 md:p-0 dark:text-white md:dark:hover:text-blue-500 dark:hover:bg-gray-700 dark:hover:text-white md:dark:hover:bg-transparent">Search</NuxtLink>
                </li>
                <li>
                <NuxtLink exact to="/popular" exact-active-class="text-blue-700" class="block py-2 px-3 text-gray-900 rounded hover:bg-gray-100 md:hover:bg-transparent md:border-0 md:hover:text-blue-700 md:p-0 dark:text-white md:dark:hover:text-blue-500 dark:hover:bg-gray-700 dark:hover:text-white md:dark:hover:bg-transparent">Popular</NuxtLink>
                </li>
                <li>
                <NuxtLink exact to="/now-playing" exact-active-class="text-blue-700" class="block py-2 px-3 text-gray-900 rounded hover:bg-gray-100 md:hover:bg-transparent md:border-0 md:hover:text-blue-700 md:p-0 dark:text-white md:dark:hover:text-blue-500 dark:hover:bg-gray-700 dark:hover:text-white md:dark:hover:bg-transparent">Now Playing</NuxtLink>
                </li>
                <li>
                <NuxtLink exact to="/top-rated" exact-active-class="text-blue-700" class="block py-2 px-3 text-gray-900 rounded hover:bg-gray-100 md:hover:bg-transparent md:border-0 md:hover:text-blue-700 md:p-0 dark:text-white md:dark:hover:text-blue-500 dark:hover:bg-gray-700 dark:hover:text-white md:dark:hover:bg-transparent">Top Rated</NuxtLink>
                </li>
                <li>
                <NuxtLink exact to="/upcoming" exact-active-class="text-blue-700" class="block py-2 px-3 text-gray-900 rounded hover:bg-gray-100 md:hover:bg-transparent md:border-0 md:hover:text-blue-700 md:p-0 dark:text-white md:dark:hover:text-blue-500 dark:hover:bg-gray-700 dark:hover:text-white md:dark:hover:bg-transparent">Upcoming</NuxtLink>
                </li>
            </ul>
            </div>
        </div>
        </nav>

        <main>

            <slot/>
        </main>

    </div>
</template>