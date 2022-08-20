<template>
    <div id="header" class="bg-[url('/menu-page.jpg')] px-20">
      <div id="menu" class="grid grid-cols-2 py-5">
        <div id="menu_left">
          <img src="logo.png" class="w-[150px]" />
          <h1 class="text-white font-oswald uppercase text-6xl text-center pt-24 pb-28">Shopping Cart</h1>
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

      <table>
        <thead>
            <tr>
                <th>Name</th>
                <th>Price</th>
                <th>Quantity</th>
                <th>Total</th>
                <th>Remove</th>
            </tr>
        </thead>
        <tbody>
            <tr v-for="order in $store.state.orders" :key="order.name">
                <td>{{ order.name }}</td>
                <td>RM {{ order.price }}</td>
                <td>{{ order.quantity }}</td>
                <td>{{ (order.price * order.quantity) }}</td>
                <td><button> ❌ </button></td>
            </tr>
        </tbody>
      </table>
    </div>
</template>
