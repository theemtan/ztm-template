<template>
  <div class="border rounded-md border-gray-200 text-left pb-5 mb-5 pl-5">
    <img :src="image" width="600" height="400" class="px-5 py-5" alt="burgers" />
    <h3 class="font-oswald font-medium text-2xl uppercase text-gray-500 mt-5 mb-2 ml-5">{{ title }}</h3>
    <p class="font-light text-gray-500 mb-5 ml-5">{{ description }}</p>
    <span class="bg-amber-800 text-yellow-300 font-bold font-oswald text-xl ml-5 rounded-lg px-5 py-2">{{ price }}</span>
  </div>
</template>

<script>
export default {
  props: ['image', 'title', 'description', 'price'],
};
</script>
