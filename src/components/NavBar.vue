<template>
    <nav>
        <!-- desktop menu --->
        <div class="bg-blue-950">
            <div class="max-w-10xl mx-auto">
                <div class="flex justify-between">
                    <!-- menu-->
                    <div class="text-white flex space-x-4">
                        <!-- logo-->
                        <div class="flex items-center space-x-2 py-5 px-2">
                            <img src="../assets/emmlogo.png" alt="emm logo" class="emm pr-2">
                            <span class="font-extrabold text-yellow-600 text-2xl">EMM</span>
                        </div>
                        <!-- menu-->
                        <div class="hidden md:flex items-center space-x-1">
                            <a href="" class="py-5 px-2 text-white hover:text-yellow-600">Home</a>
                            <a href="" class="py-5 px-2 text-white hover:text-yellow-600">About</a>
                            <a href="" class="py-5 px-2 text-white hover:text-yellow-600">Contact</a>
                            <a href="" class="py-5 px-2 text-white hover:text-yellow-600">Resources</a>
                        </div>
                    </div>
                    <!-- register-->
                    <div class="hidden md:flex items-center space-x-1">
                        <button class="mr-4 bg-yellow-600 bg-opacity-70 hover:bg-yellow-300 text-white font-bold py-2 px-4 rounded">
                            Register
                        </button>
                        <button class="ml-4 bg-transparent hover:bg-yellow-300 text-white font-semibold hover:text-white py-2 px-4 border border-yellow-600 hover:border-transparent rounded">
                            Login
                        </button>
                    </div>
                    <!-- botton to show mobile menu-->
                    <div class="flex items-center md:hidden">
                        <button @click="showMobileMenu = !showMobileMenu" class="text-white py-5 px-2"><i class="fa fa-list h-8 w-8"></i></button>
                    </div>
                </div>
            </div>
        </div>

        <!-- mobile menu --->
        <div class="md:hidden bg-blue-950 text-left" :class="{ hidden: showMobileMenu }">
            <a href="" class="block py-2 px-4 hover:bg-blue-900 hover:text-blue-400 text-blue-200">Home</a>
            <a href="" class="block py-2 px-4 hover:bg-blue-900 hover:text-blue-400 text-blue-200">About</a>
            <a href="" class="block py-2 px-4 hover:bg-blue-900 hover:text-blue-400 text-blue-200">Contact</a>
            <a href="" class="block py-2 px-4 hover:bg-blue-900 hover:text-blue-400 text-blue-200">Resources</a>

            <div class="md:hidden p-4" :class="{ hidden: showMobileMenu }" >
                <button class="bg-yellow-600 bg-opacity-70 hover:bg-yellow-300 text-white mr-3 font-bold py-2 px-4 rounded">
                    Register
                </button>
                <button class="bg-transparent hover:bg-yellow-300 text-white font-semibold hover:text-white py-2 px-4 border border-yellow-600 hover:border-transparent rounded">
                    Login
                </button>
            </div>
        </div>
    </nav>
    <div class="p-8 text-2xl font-extremebold text-center">
        Content
    </div>
</template>

<script setup>
    import { ref } from "vue";

    const showMobileMenu = ref(true);
</script>

<style scoped>
    .emm {
        height: 40px;
        width: 50px;
    }
    .rounded {
        border-radius: 100px;
        width: 150px;
        opacity: 100;
    }
</style>
