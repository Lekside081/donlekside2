<template>
    <div class="mt-24">
        <div class="flex justify-center mb-24">
            <div class="basis-11/12 bg-yellow-500 rounded-3xl py-20">
                <div>
                    <p class="font-bold text-5xl text-center">Ready to
                        <span>Go Borda-less<span class="">
                                <div class="flex justify-center -mt-8 ml-60">
                                    <div class="mt-8 bg-local h-5 w-52"
                                        style="background-image: url('/underline.svg'); background-size: cover; background-position: center;">
                                    </div>
                                </div>
                            </span></span>
                    </p>
                    <p class="text-center mt-6">Send, receive, convert, and manage multiple currencies in one</p>
                    <p class="text-center">platform.</p>
                    <div class="flex justify-center mt-8">
                        <button class="bg-blue-900 text-sm font-bold py-3 text-white px-5 rounded-full">
                            Get Started!
                        </button>
                    </div>
                </div>
            </div>
        </div>
        <p class="text-5xl font-bold text-center mb-24">Frequently Asked Questions</p>

        <div class="mx-auto bg-gray-200 my-4 w-[60%] rounded-lg">
            <div class="cursor-pointer py-4" @click="PaybordaMenu = !PaybordaMenu">
                <div class="flex justify-between px-4">
                    <p class="font-bold">What is Payborda?</p>
                    <div>
                        <svg class="w-[34px] h-[34px] text-gray-800 dark:text-white bg-green-400 rounded-full py-2 px-2" aria-hidden="true"
                            xmlns="http://www.w3.org/2000/svg" width="24" height="24" fill="none" viewBox="0 0 24 24">
                            <path stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                                d="M12 19V5m0 14-4-4m4 4 4-4" />
                        </svg>
                    </div>
                </div>
            </div>
            <BodyFaqcontrol v-show="PaybordaMenu" />
        </div>

        <div class="mx-auto bg-gray-200 my-4 w-[60%] rounded-lg">
            <div class="cursor-pointer py-4" @click="VirtualMenu = !VirtualMenu">
                <div class="flex justify-between px-4">
                    <p class="font-bold">How does the Virtual Account Work?</p>
                    <div>
                        <svg class="w-[34px] h-[34px] text-gray-800 dark:text-white bg-green-400 rounded-full py-2 px-2" aria-hidden="true"
                            xmlns="http://www.w3.org/2000/svg" width="24" height="24" fill="none" viewBox="0 0 24 24">
                            <path stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                                d="M12 19V5m0 14-4-4m4 4 4-4" />
                        </svg>
                    </div>
                </div>
            </div>
            <BodyFaqcontrol2 v-show="VirtualMenu" />
        </div>

        <div class="mx-auto bg-gray-200 my-4 w-[60%] rounded-lg">
            <div class="cursor-pointer py-4" @click="Payborda2Menu = !Payborda2Menu">
                <div class="flex justify-between px-4">
                    <p class="font-bold">How do I Place an FX Bid on PayBorda?</p>
                    <div>
                        <svg class="w-[34px] h-[34px] text-gray-800 dark:text-white bg-green-400 rounded-full py-2 px-2" aria-hidden="true"
                            xmlns="http://www.w3.org/2000/svg" width="24" height="24" fill="none" viewBox="0 0 24 24">
                            <path stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                                d="M12 19V5m0 14-4-4m4 4 4-4" />
                        </svg>
                    </div>
                </div>
            </div>
            <BodyFaqcontrol3 v-show="Payborda2Menu" />
        </div>

        <div class="mx-auto bg-gray-200 my-4 w-[60%] rounded-lg">
            <div class="cursor-pointer py-4" @click="Payborda3Menu = !Payborda3Menu">
                <div class="flex justify-between px-4">
                    <p class="font-bold">What Fees are Charged for Using PayBorda?</p>
                    <div>
                        <svg class="w-[34px] h-[34px] text-gray-800 dark:text-white bg-green-400 rounded-full py-2 px-2" aria-hidden="true"
                            xmlns="http://www.w3.org/2000/svg" width="24" height="24" fill="none" viewBox="0 0 24 24">
                            <path stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                                d="M12 19V5m0 14-4-4m4 4 4-4" />
                        </svg>
                    </div>
                </div>
            </div>
            <BodyFaqcontrol4 v-show="Payborda3Menu" />
        </div>
    </div>
</template>

<script setup lang="ts">
const PaybordaMenu = ref(false)

const VirtualMenu = ref(false)

const Payborda2Menu = ref(false)

const Payborda3Menu = ref(false)
</script>