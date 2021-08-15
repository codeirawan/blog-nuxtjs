<template>
    <!-- header -->
    <header class="header my-8">
        <!-- container -->
        <div class="container px-4 sm:px-8 lg:px-16 xl:px-20 mx-auto">
            <!-- header wrapper -->
                <div class="header-wrapper flex items-center justify-between">

                    <!-- header logo -->
                    <div class="header-logo">
                        <nuxt-link to="/" class="hover:text-sky-900"><img src="https://www.yesdok.com/img/headeryesdok.png" width="80px" lg:width="150px" alt="YesDok, Konsultasi Dokter Online 24 Jam" /></nuxt-link>
                    </div>

                    <!-- mobile toggle -->
                    <div class="toggle md:hidden">
                        <button @click=" isOpen = true" @keydown.escape=" isOpen = false">
                            <svg 
                                class="h-6 w-6 fill-current text-black"
                                fill="none" stroke-linecap="round" 
                                stroke-linejoin="round" stroke-width="2" 
                                viewBox="0 0 24 24" stroke="currentColor">
                                <path d="M4 6h16M4 12h16M4 18h16"></path>
                            </svg>
                        </button>
                    </div>

                    <!-- Navbar -->
                    <navbar class="navbar hidden md:block">
                        <ul class="flex space-x-8 text-sm font-semibold">
                            <li><nuxt-link to="/posts" class="active border-b-2 border-red-700 pb-2">Blog</nuxt-link></li>
                            <li><nuxt-link to="#" class="hover:text-sky-900">Service</nuxt-link></li>
                            <li><nuxt-link to="#" class="hover:text-sky-900">About</nuxt-link></li>
                            <li><nuxt-link to="#" class="hover:text-sky-900">Career</nuxt-link></li>
                            <li><nuxt-link to="#" class="hover:text-sky-900">Contact</nuxt-link></li>
                            <li><nuxt-link to="#" class="cta bg-sky-900 hover:bg-sky-700 px-3 py-2 rounded text-white font-normal">Login</nuxt-link></li>
                        </ul>
                    </navbar>

                </div>
        </div>
    </header><!-- end header -->
</template>