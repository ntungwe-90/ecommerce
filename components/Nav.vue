<template>
  <div class="h-20 bg-[#A88686]">
   <div class="navbar flex text-white relative">
      <div class="nav-item-center flex space-x-6 sm:space-x-20 p-5 mx-auto text-lg ">
        <NuxtLink to="/" class="hover:bg-pink-300 hover:text-black  hover:rounded ">Home</NuxtLink>
        <NuxtLink to="/men" class="hover:bg-pink-300 hover:text-black  hover:rounded ">Men</NuxtLink>
        <NuxtLink to="/women" class="hover:bg-pink-300 hover:text-black  hover:rounded ">Women</NuxtLink>
        <NuxtLink to="/all" class="hover:bg-pink-300 hover:text-black  hover:rounded ">All</NuxtLink>
        <nuxt-link to="/cart"><svg xmlns="http://www.w3.org/2000/svg" width="25" height="25" fill="currentColor" class="bi bi-cart4" viewBox="0 0 16 16">
  <path d="M0 2.5A.5.5 0 0 1 .5 2H2a.5.5 0 0 1 .485.379L2.89 4H14.5a.5.5 0 0 1 .485.621l-1.5 6A.5.5 0 0 1 13 11H4a.5.5 0 0 1-.485-.379L1.61 3H.5a.5.5 0 0 1-.5-.5zM3.14 5l.5 2H5V5H3.14zM6 5v2h2V5H6zm3 0v2h2V5H9zm3 0v2h1.36l.5-2H12zm1.11 3H12v2h.61l.5-2zM11 8H9v2h2V8zM8 8H6v2h2V8zM5 8H3.89l.5 2H5V8zm0 5a1 1 0 1 0 0 2 1 1 0 0 0 0-2zm-2 1a2 2 0 1 1 4 0 2 2 0 0 1-4 0zm9-1a1 1 0 1 0 0 2 1 1 0 0 0 0-2zm-2 1a2 2 0 1 1 4 0 2 2 0 0 1-4 0z"/>
</svg></nuxt-link>
      </div> 
      <div class="cart fixed bottom-0 right-0 shadow-md m-3">
        <p class="p-1 cartCount text-xs absolute top-0 right-0">
         
        </p>
        <NuxtLink to="/cart">
          <p class="pt-3 px-2">Cart</p>
        </NuxtLink>
      </div>
      <!-- <div class="ham-menu shadow-md fixed bottom-0 right-0 m-3 sm:hidden">
        <p class="text-center pt-3">menu</p>
      </div> -->
    </div>
   
  </div>
  </template>
  
  <script>
  
  export default {
    name: 'Nav',
   
  }
  </script>
  
  <style scoped>
  .ham-menu {
    background-color: #000;
    width: 3em;
    height: 3em;
    border-radius: 1.5em;
  }
  .cart {
    background-color: rgb(163, 87, 129);
    width: 3em;
    height: 3em;
    border-radius: 1.5em;
  }
  .navbar {
    background-color: rgb(24, 20, 22);
  }
  .cartCount {
    background: #000;
    border-radius: 30%;
  }
  </style>