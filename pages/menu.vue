<template>
  <div>
    <div id="header" class="bg-[url('/menu-page.jpg')] px-20">
      <div id="menu" class="grid grid-cols-2 py-5">
        <div id="menu_left">
          <img src="'/'+logo.png" class="w-[150px]" />
          <h1 class="text-white font-oswald uppercase text-6xl text-center pt-24 pb-28">Our Menu</h1>
        </div>

        <div id="menu_right">
          <ul class="grid grid-cols-5 text-lg font-papyrus text-white uppercase pt-5">
            <li>About Us</li>
            <NuxtLink to="/menu">Our Menu</NuxtLink>
            <li>Contact Us</li>
            <li>Location</li>
            <NuxtLink to="/cart">Cart ({{ $store.getters.totalItems }})</NuxtLink>
          </ul>
        </div>
      </div>
    </div>
    <div id="items" class="grid grid-cols-3 gap-x-5 gap-y-16 mt-10 mx-20">
      <MenuItem v-for="b in items" :key="b.name" :item="b" />
    </div>
  </div>
</template>
<!-- load data , data method -->
<!-- return variable -->
<!-- mounted method - when component is loaded -->
<!-- axios is a library -->

<script>
export default {
  data() {
    return {
      items: [],
    };
  },
  mounted() {
    this.$axios.get('items.json').then(
      (response) => {
        this.items = response.data.burgers;
      });
  },
};
</script>
