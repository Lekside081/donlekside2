<template>
  <div class="bg-gray-100 py-6">
    <div class="flex items-center justify-between px-4 lg:px-10">
      <div class="basis-1/4">
        <p class="font-bold text-2xl">Donlekside</p>
      </div>

      <div class="hidden sm:flex basis-1/2 justify-between">
        <div class="flex space-x-4">
          <div class="cursor-pointer flex items-center" @click="featureMenu = !featureMenu">
            Feature
            <svg class="w-[17px] h-[17px] text-gray-800 dark:text-white ml-1" xmlns="http://www.w3.org/2000/svg"
              width="24" height="24" fill="none" viewBox="0 0 24 24">
              <path stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                d="m19 9-7 7-7-7" />
            </svg>
          </div>
          <NuxtLink to="/" class="cursor-pointer mt-1">Pricing</NuxtLink>
          <NuxtLink to="/events" class="cursor-pointer mt-1">Events</NuxtLink>
          <UDropdown v-model:open="open" class="font-bold cursor-pointer" :items="items"
            :popper="{ placement: 'bottom-start', width: 'w-1/5' }">
            <UButton class="bg-gray-100 text-black hover:bg-gray-100" label="Learn"
              trailing-icon="i-heroicons-chevron-down-20-solid" />
          </UDropdown>
          <UDropdown v-model:open2="open2" class="font-bold cursor-pointer" :items="items2"
            :popper="{ placement: 'bottom-start', width: 'w-1/5' }">
            <UButton class="bg-gray-100 text-black hover:bg-gray-100" label="Company"
              trailing-icon="i-heroicons-chevron-down-20-solid" />
          </UDropdown>
        </div>
      </div>

      <div class="hidden sm:flex basis-1/4 justify-end space-x-6">
        <button class="bg-green-200 hover:bg-green-300 font-bold py-2 px-4 rounded-full">
          Register
        </button>
        <input type="text" placeholder="Login"
          class="text-center font-bold w-24 border border-gray-800 bg-gray-100 rounded-full py-2" />
        <svg class="w-8 h-8 text-gray-800 dark:text-white" xmlns="http://www.w3.org/2000/svg" width="24" height="24"
          fill="none" viewBox="0 0 24 24">
          <path stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
            d="M18.427 14.768 17.2 13.542a1.733 1.733 0 0 0-2.45 0l-.613.613a1.732 1.732 0 0 1-2.45 0l-1.838-1.84a1.735 1.735 0 0 1 0-2.452l.612-.613a1.735 1.735 0 0 0 0-2.452L9.237 5.572a1.6 1.6 0 0 0-2.45 0c-3.223 3.2-1.702 6.896 1.519 10.117 3.22 3.221 6.914 4.745 10.12 1.535a1.601 1.601 0 0 0 0-2.456Z" />
        </svg>
      </div>
    </div></div>

    <div v-show="featureMenu" class="border mx auto w-[40%]">
      <HeadNavFaq />
    </div>
</template>

<script setup lang="ts">

const featureMenu = ref(false);

const items = [
  [{ label: "Blog", avatar: { src: "https://avatars.githubusercontent.com/u/739984?v=4" } }],
  [{ label: "Resources", avatar: { src: "https://avatars.githubusercontent.com/u/739984?v=4" } }],
];

const open = ref(false);

const items2 = [
  [{ label: "About Us", avatar: { src: "https://avatars.githubusercontent.com/u/739984?v=4" } }],
  [{ label: "Careers", avatar: { src: "https://avatars.githubusercontent.com/u/739984?v=4" } }],
];

const open2 = ref(false);

const toggleFeatureMenu = () => {
  featureMenu.value = !featureMenu.value;
};
</script>
