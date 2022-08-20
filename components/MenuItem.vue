<template>
  <div class="border rounded-md border-gray-200 text-center py-5 mb-5 pl-5">
    <div>
      <img :src="'/'+item.image" width="500" height="200" class="border border-gray p-5" alt="burgers" />
    </div>
    <h4 class="font-oswald text-2xl uppercase mt-5">{{ item.name }}</h4>
    <p class="font-light text-gray-500 my-2">{{ item.description }}</p>
    <p class="mt-5 mb-8">
      <span class="rounded rounded-lg bg-amber-800 text-yellow-400 font-bold font-oswald text-xl ml-5 px-5 py-2">{{ item.price.toFixed(2) }}</span>
    </p>
    <button class="button font-oswald uppercase border py-2 px-3" @click="addItem">Add to Cart</button>
  </div>
</template>

<script>
export default {
  props: ['item'],
  methods: {
    addItem() {
      this.$store.commit('addItem', this.item);
    },
  },
};
</script>
