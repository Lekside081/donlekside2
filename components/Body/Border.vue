<template>
    <div class="mt-14 px-4 sm:px-10">
      <!-- Header Section -->
      <div>
        <p class="text-center text-4xl sm:text-6xl font-bold">
          Borda-less Payments at
        </p>
        <p class="text-center text-4xl sm:text-6xl font-bold">Your Fingertips</p>
        <p class="text-lg sm:text-xl text-center mt-4">
          Send and Receive Payments without boundaries locally and internationally
        </p>
        <p class="text-lg sm:text-xl text-center">
          with PayBorda! Enjoy simplified payment solutions made for you.
        </p>
      </div>
  
      <!-- Buttons Section -->
      <div class="flex flex-col sm:flex-row justify-center space-y-4 sm:space-y-0 sm:space-x-6 mt-6">
        <button class="bg-blue-900 hover:bg-blue-500 text-white font-bold py-3 px-6 rounded-full w-full sm:w-auto">
          Create a Free Account
        </button>
        <input
          id="demo-request"
          type="text"
          placeholder="Request a Demo"
          class="text-center font-bold w-full sm:w-auto border border-gray-800 bg-gray-100 hover:bg-gray-200 rounded-full py-3"
        />
      </div>
  
      <!-- Hero Image -->
      <div
        class="mt-8 bg-local h-72 sm:h-screen w-full sm:w-1/2 mx-auto"
        style="background-image: url('/home-hero-img.png'); background-size: cover; background-position: center;"
      ></div>
  
      <!-- Endless Payment Possibilities Section -->
      <div class="py-10">
        <p class="font-bold text-3xl sm:text-5xl text-center">
          Endless Payment Possibilities.
        </p>
        <p class="font-bold text-3xl sm:text-5xl text-center mt-4">
          Go Borda-less
        </p>
        <div class="flex justify-center mt-2">
          <div
            class="bg-local h-2 w-40 sm:w-52"
            style="background-image: url('/underline.svg'); background-size: cover; background-position: center;"
          ></div>
        </div>
      </div>
  
      <!-- Description Section -->
      <div class="mb-10 sm:mb-40 text-center px-4">
        <p class="text-lg sm:text-xl">
          With PayBorda, your business can effortlessly navigate the global
          landscape while embracing new opportunities with no restrictions.
        </p>
      </div>
  
      <!-- Features Section -->
      <div class="flex flex-col sm:flex-row justify-center items-center space-y-8 sm:space-y-0 sm:space-x-10 px-4 mb-10">
        <div class="basis-full sm:basis-1/3 text-center sm:text-left">
          <div class="mb-4">
            <span class="bg-white font-bold py-2 px-4 rounded-full border text-blue-300">
              Seamless Payment
            </span>
          </div>
          <p class="font-bold text-2xl sm:text-3xl mt-2">
            Borda-less Payments
          </p>
          <p class="mt-4">
            Send, Receive, and Manage Multiple Currencies with Ease. Make
            payments in minutes. Manage and process international payments in
            multiple currencies from a single dashboard.
          </p>
          <div class="flex flex-col sm:flex-row space-y-4 sm:space-y-0 sm:space-x-4 mt-6">
            <button class="bg-blue-900 text-white font-bold py-3 px-5 rounded-full w-full sm:w-auto">
              Make a Conversion
            </button>
            <button class="bg-white font-bold py-3 px-5 rounded-full border text-blue-900 w-full sm:w-auto">
              Learn More
            </button>
          </div>
        </div>
        <div class="basis-full sm:basis-1/3">
          <div
            class="bg-local h-64 sm:h-72 w-72"
            style="background-image: url('/transfers1.png'); background-size: cover; background-position: center;"
          ></div>
        </div>
      </div>
  
      <!-- Best Rate Section -->
      <div class="flex flex-col sm:flex-row justify-center items-center space-y-8 sm:space-y-0 sm:space-x-10 px-4 mt-20">
        <div class="basis-full sm:basis-1/3">
          <div
            class="bg-local h-64 sm:h-96 w-72"
            style="background-image: url('/Weightlose.jpg'); background-size: cover; background-position: center;"
          ></div>
        </div>
        <div class="basis-full sm:basis-1/3 text-center sm:text-left">
          <span class="bg-white font-bold py-2 px-4 rounded-full border text-red-400">
            Best Rate
          </span>
          <p class="font-bold text-2xl sm:text-3xl mt-4">
            Bid Affordable FX
          </p>
          <p class="mt-4">
            Secure the Best FX Rates in USD, EUR, and GBP. Unlock premium FX rates
            in USD, EUR, and GBP. Bid smart, save big, and watch your business
            thrive with every conversion.
          </p>
          <div class="mt-6">
            <button class="bg-blue-900 text-white font-bold py-3 px-5 rounded-full w-full sm:w-auto">
              Start Your Bid
            </button>
          </div>
        </div>
      </div>
    </div>
  </template>
  
  <script setup>
  defineProps(['img']);
  </script>
  