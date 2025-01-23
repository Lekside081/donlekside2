<template>
  <div class="mb-40 flex flex-col sm:flex-row justify-center  space-y-4 sm:space-y-0 sm:space-x-6 mt-20">
    <UCarousel v-slot="{ item, index }" :items="students" :ui="{ item: 'w-10/12 h-'}">
        <div class="basis-11/12 rounded-3xl ml-16" :class="item.color">
          <div class="flex">
            <div class="basis-8/12 py-8 mt-10">
              <p class="font-bold text-3xl ml-14">{{ item.name }}</p>
              <div class="flex justify-center">
                <div class="basis-11/12 ml-5 mt-2 rounded-3xl">
                  <p class="ml-5 font-bold">{{ item.descreption }}</p>
                  <p class="ml-5 font-bold">{{ item.descreption2 }}</p>
                  <p class="ml-5 font-bold">{{ item.descreption3 }}</p>
                  <div class="ml-4 m-6">
                    <text class="bg-gray-200 text-sm py-2 text-gray-800 px-4 rounded-full border border-black">
                      Learn More
                  </text>
                </div>

                </div>
              </div>
            </div>
            <div class="basis-5/12">
              <div class="flex justify-center">
                <div class="basis-10/12 rounded-3xl mt-8">
                  <div class="m-8" :class="item.img">
                    <div><img :src="item.avatar.src"></div>
                  </div>
                </div>
              </div>
            </div>
          </div>
        </div>
    </UCarousel>
    </div>

    <div class="ml-20 mb-6">
      <p class="text-4xl font-bold">We asked our customers how likely</p>
      <p class="text-4xl font-bold">they are to recommend PayBorda</p>
      <div class="mt-4">
        <button class="bg-blue-900 text-sm font-bold py-3 text-white px-6 rounded-full">
            Tell Us Your Story!
        </button>
    </div>
    </div>
    </template>
    <script setup lang="ts">
  const students = [{
    name: 'Perks and Discount',
    color: 'bg-gray-200',
    descreption: 'Unlock exclusive discounts on insurance, legal',
    descreption2: 'services, office space, and more. With PayBorda,',
    descreption3: 'your business saves on what matters most.',
    avatar: { src: '/transfers1.png' }
  }, {
    name: 'Events',
    color: 'bg-gray-200',
    descreption: 'Host your events, handle payments in multiple',
    descreption2: 'currencies, and pay vendors—all from a single',
    descreption3: 'app.',
    avatar: { src: '/cards4.png' }
  }, {
    name: 'Team Management',
    color: 'bg-gray-200',
    descreption: 'Manage payments and transactions and simplify',
    descreption2: 'team collaboration—no matter where you',
    descreption3: 'employees are.',
    avatar: { src: 'convert3.png' }
  },]
  </script>
  