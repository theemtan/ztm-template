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

    <div id="section-1" class="text-center bg-[url('/bg-burgers.png')] py-40 bg-cover">
    <h1 class="text-6xl uppercase font-oswald pt-20 px-24">
      The burger tastes better when you eat it with family
    </h1>

    <p class="font-roboto font-light text-lg py-6 px-28">
      Spend quality time with your family and eat an affordable, nutritious and delicious meal together.
      Not all burgers are fast foods. All our burgers are handmade to order for your family members to enjoy.
    </p>

    <button class="font-oswald uppercase bg-red-500 text-white py-3 px-8">
      Explore Full Menu
    </button>
    </div>

    <div id="section-2" class="bg-yellow-500 py-10 px-20">
      <div class="grid grid-cols-3 text-center text-neutral-900 xl:px-52">
        <div>
          <svg xmlns="http://www.w3.org/2000/svg" class="h-20 w-20 block mx-auto" fill="none" viewBox="0 0 24 24" stroke="currentColor">
            <path stroke-linecap="round" stroke-linejoin="round" d="M5 3v4M3 5h4M6 17v4m-2-2h4m5-16l2.286 6.857L21 12l-5.714 2.143L13 21l-2.286-6.857L5 12l5.714-2.143L13 3z" />
          </svg>
          <p class="font-medium font-oswald text-2xl uppercase my-5">Original Recipes</p>
          <p class="font-light font-roboto px-5">
          We use our secret recipes with only the best ingredients to make our burgers.
          Starting from patties, sauces, and even buns.
        </p>
        </div>

        <div>
          <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke="currentColor" class="h-20 w-20 block mx-auto">
            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="1" d="M21 15.546c-.523 0-1.046.151-1.5.454a2.704 2.704 0 01-3 0 2.704 2.704 0 00-3 0 2.704 2.704 0 01-3 0 2.704 2.704 0 00-3 0 2.704 2.704 0 01-3 0 2.701 2.701 0 00-1.5-.454M9 6v2m3-2v2m3-2v2M9 3h.01M12 3h.01M15 3h.01M21 21v-7a2 2 0 00-2-2H5a2 2 0 00-2 2v7h18zm-3-9v-2a2 2 0 00-2-2H8a2 2 0 00-2 2v2h12z" />
          </svg>
          <p class="font-medium font-oswald text-2xl uppercase my-5">Quality Foods </p>
          <p class="font-light font-roboto px-5">
          We purchase our ingredients from the best suppliers daily, to ensure the freshest quality of our burgers.
          </p>
        </div>

        <div>
          <svg xmlns="http://www.w3.org/2000/svg" class="h-20 w-20 block mx-auto" fill="none" viewBox="0 0 24 24" stroke="currentColor">
            <path stroke-linecap="round" stroke-linejoin="round" d="M13 10V3L4 14h7v7l9-11h-7z" />
          </svg>
          <p class="font-medium font-oswald text-2xl uppercase my-5">Fastest Delivery</p>
          <p class="font-light font-roboto px-5">
          Burgers are best served while it's hot. We deliver to your door with our
          speedy delivery partners from the nearest outlet.
          </p>
        </div>
      </div>
    </div>

    <div id="section-3" class="text-center">
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

      <div id="section-4" class="grid grid-cols-12 font-oswald uppercase text-4xl text-yellow-800 px-40 gap-5">
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
      <div id="section-4a" class="grid grid-cols-3 px-40 mt-5 gap-5">
        <img src="offer-1.jpg" alt="">
        <img src="offer-2.jpg" alt="">
        <img src="offer-3.jpg" alt="">
      </div>
      <div id="section-4b" class="px-20">
      <div class="grid grid-cols-2 bg-gray-200 px-20 py-20">
        <img src="about.png" alt="" class="pl-20">
        <h3 class="font-oswald text-6xl uppercase pl-20 pr-4 pt-40 leading-snug">
        Nothing Brings <br />
        People Together Like A <br />
        Good Burger!!! <br />
        </h3>
      </div>
        <p class="text-xl text-gray-500 mt-10">
          That's the philosophy that we always believe in. We're a family-owned and operated business, and we're proud to be a part of the community.We do our best to make sure that everyone's happy and having a good time.
        </p>
        <p class="text-xl text-gray-500 mb-20">
          Burgers are what brought us together and what keeps us together. It's something that you can't put a price tag on. More importantly, we are interested in people. It's not just about the food.
        </p>
      </div>
        <div id="section-5" class="grid grid-cols-5 bg-yellow-500 text-amber-900">
          <div class="col-span-3 pl-20 pt-16 pb-16 text-center">
            <h4 class="font-oswald text-5xl">
            Download Mobile App
            </h4>
            <h4 class="font-oswald text-6xl uppercase">
            Save up to 20%
            </h4>
            <p class="text-lg my-7">
            Bye bye long queues. Order before and your food will be ready in a flash.
            <br />
            Enjoy the convenience of ordering food online at any time and from any location.
            </p>
            <button><img src="appstore.png" alt="" class="h-[50px]"></button> <button><img src="googleplay.png" alt="" class="h-[50px]"></button>
          </div>
          <div class="col-span-2">
            <img src="eshop.png" alt="" class="-mt-10 h-[500px] object-cover">
          </div>
        </div>
    </div>
    </div>
  </div>
</template>
