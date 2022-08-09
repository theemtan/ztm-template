<template>
  <div>
  <div id="header" class="bg-[url('/hero-bg.jpg')] px-20">
    <div id="menu" class="grid grid-cols-2 py-5">
      <div id="menu_left">
        <img src="logo.png" class="w-[150px]" />
      </div>

      <div id="menu_right">
        <ul class="grid grid-cols-4 text-lg font-papyrus text-white uppercase pt-5">
          <li>About Us</li>
          <li>Our Menu</li>
          <li>Contact Us</li>
          <li>Location</li>
        </ul>
      </div>
    </div>

    <div class="grid grid-cols-2 pb-20 pt-10">
      <img src="hero-burger.png" class="pr-8 mt-10" alt="" />
      <div>
        <h1 class="text-9xl text-white text-center font-lilita uppercase"> Classic Burger</h1>
        <h2 class="text-7xl text-white text-center font-lilita uppercase my-5">With Onion</h2>
        <p class="text-2xl text-white font-roboto font-light text-center pt-10"> Our Signature Burger now comes with onion and cheese. You can customise it to your liking. Freshly made to order, all in a brioche style bun. </p>
      </div>
    </div>
    </div>
    <div id="section-1" class="text-center bg-[url('/burger-bg-1.jpg')] pb-80 bg-cover">
      <h1 class="text-6xl text-black text-center font-roboto uppercase pt-20 px-24">The burger tastes better when you eat it with family</h1>
      <p class="text-black text-center font-roboto text-lg py-6 px-28">Spend quality time with your family and eat an affordable , nutritious and delicious meal together.</p>
      <button class="font-oswald uppercase bg-red-500 text-white text-center py-3 px-8">Explore Full Menu</button>
    </div>
    <div id="section-2" class="text-center">
      <h2 class="text-6xl font-oswald text-red-500 uppercase font-medium pt-20">Our Crazy Burgers</h2>
      <p class="text-gray-500 font-light text-x1 my-10 px-20">Whether you are looking for Classics, our specialties or just wraps, salads and fries. We have it all. We always have something that rewards your tastebuds</p>

    <div class="grid grid-cols-2 px-80 gap-5">
        <div id="left-item-column">
          <Item />
          <Item />
        </div>
        <div id="right-item-column">
          <Item />
        </div>
    </div>
    </div>
  </div>
</template>
