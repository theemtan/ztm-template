<template>
  <div>
  <div id="header" class="bg-[url('/hero-bg.jpg')] px-20">
    <div id="menu" class="grid grid-cols-2 py-5">
      <div id="menu_left">
        <img src="logo.png" class="w-[150px]" />
      </div>

      <div id="menu_right">
        <ul class="grid grid-cols-5 text-lg font-papyrus text-white uppercase pt-5">
          <li>About Us</li>
          <NuxtLink to="/menu">Our Menu</NuxtLink>
          <li>Contact Us</li>
          <li>Location</li>
          <NuxtLink to="/cart">Cart</NuxtLink>
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

    <div id="section-1" class="text-center bg-[url('/three_burgers.jpg')] pb-96 bg-cover">
    <h1 class="text-6xl uppercase font-oswald pt-20 px-24">
      The burger tastes better when you eat it with family
    </h1>

    <p class="font-roboto font-light text-gray-500 text-lg py-6 px-28">
      Spend quality time with your family and eat an affordable, nutritious and delicious meal together.
      Not all burgers are fast foods. All our burgers are handmade to order for your family members to enjoy.
    </p>

    <button class="font-oswald uppercase bg-red-500 text-white py-3 px-8">
      Explore Full Menu
    </button>
    </div>

    <div id="section-2" class="text-center">
      <h2 class="text-6xl font-oswald text-red-500 uppercase font-medium pt-20">Our Crazy Burgers</h2>
      <p class="text-gray-500 font-light text-x1 my-10 px-20">Whether you are looking for Classics, our specialties or just wraps, salads and fries. We have it all. We always have something that rewards your tastebuds</p>
    </div>

    <div class="grid grid-cols-2 px-80 gap-5">
        <div id="left-item-column">
          <Item image="crispy-chicken.jpg" title="Crispy Chicken Burger" description="Chicken Breast, Chilli Sauce, Tomatoes, Pickles, Coleslaw" price="11.99" />
          <Item image="double-burger.jpg" title="Double Cheeseburger" description="Aussie Beef Patty, Barbeque Sauce, Crispy Bacon, Red Onions" price="16.99" />
        </div>
        <div id="right-item-column">
          <Item image="baa-baa.jpg" title="Baa Baa Black Sheep" description="Juicy Lamb Patty, American Cheese, Tomato Relish, Lettuce" price="15.75" />
          <Item image="ultimate-bacon.jpg" title="Ultimate Bacon" description="House Beef Patty, Cheddar Cheese, Smokey Bacon, Onions, Mustard" price="14.99" />
        </div>
    </div>

      <div id="section-3" class="grid grid-cols-12 font-oswald uppercase text-4xl text-yellow-800 px-40 gap-5">
        <div class="col-span-5 bg-cover bg-center bg-[url('/fries-bg-1.jpg')] text-right pl-20 pb-10 pt-10 pr-10">
          <h4>Get Your free</h4>
          <h4>Cheese Fries</h4>
          <button class="uppercase bg-red-500 text-white text-lg py-3 px-8 mt-5">Claim Now</button>
        </div>
        <div class="col-span-7 bg-cover bg-center bg-[url('/burger-bg-1.jpg')] text-right pr-10 pt-10">
          <h4>
          Crispy <br />
          Chicken
          </h4>
          <h4>
            Burger <br />
            is back!
          </h4>
          <button class="uppercase bg-red-500 text-white text-lg py-3 px-8 mt-5">Claim Now</button>
        </div>
      </div>
      <div id="section-4" class="grid grid-cols-3 px-40 mt-5 gap-5"><img src="offer-1.jpg" alt=""> <img src="offer-2.jpg" alt=""> <img src="offer-3.jpg" alt=""></div>
    </div>
  </div>
</template>
