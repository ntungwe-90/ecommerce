<template>
 <div>   
 <header
  class="relative flex items-center justify-center h-screen mb-12 overflow-hidden"
>
  <div
    class="relative z-30 p-5 text-2xl text-white bg-purple-300 bg-opacity-50 rounded-xl"
  >
    Welcome to my site!
  </div>
  <video
    autoplay
    loop
    muted
    class="absolute z-10 w-auto min-w-full min-h-full max-w-none"
  >
    <source
      src="../static/imgs/pexels-kindel-media-6994619.mp4"
      type="video/mp4"
    />
    Your browser does not support the video tag.
  </video>
</header>

<div class="flex justify-evenly mt-10">
   <div class="max-w-sm bg-white rounded-lg border border-gray-200 shadow-md dark:bg-gray-800 dark:border-gray-700">
    <a href="#">
        <img class="rounded-t-lg" src="../static/imgs/dom-hill-nimElTcTNyY-unsplash.jpg" alt="">
    </a>
    <div class="p-5 text-center">
        <a href="#">
            <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white">Nike Lebrown-18</h5>
        </a>
        <button type="button" class="text-green-700 bg-white border border-green-700 focus:outline-none hover:bg-green-700 focus:ring-4 focus:ring-gray-200 font-medium rounded-lg text-sm px-5 py-2.5 mr-2 mb-2 dark:bg-green-700 dark:text-white dark:border-green-700 ">View Product</button>
    </div>
</div>
<div class="max-w-sm bg-white rounded-lg border border-gray-200 shadow-md dark:bg-gray-800 dark:border-gray-700">
    <a href="#">
        <img class="rounded-t-lg" src="../static/imgs/dress.jpg" alt="">
    </a>
    <div class="p-5 text-center">
        <a href="#">
            <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white">Nike Lebrown-18</h5>
        </a>
        <button type="button" class="text-green-700 bg-white border border-green-700 focus:outline-none hover:bg-green-700 focus:ring-4 focus:ring-gray-200 font-medium rounded-lg text-sm px-5 py-2.5 mr-2 mb-2 dark:bg-green-700 dark:text-white dark:border-green-700 ">View Product</button>
    </div>
</div>
<div class="max-w-sm bg-white rounded-lg border border-gray-200 shadow-md dark:bg-gray-800 dark:border-gray-700">
    <a href="#">
        <img class="rounded-t-lg" src="../static/imgs/khaled-ghareeb-Ej0mAvW6GWM-unsplash.jpg" alt="">
    </a>
    <div class="p-5 text-center">
        <a href="#">
            <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white">Nike Lebrown-18</h5>
        </a>
        <button type="button" class="text-green-700 bg-white border border-green-700 focus:outline-none hover:bg-green-700 focus:ring-4 focus:ring-gray-200 font-medium rounded-lg text-sm px-5 py-2.5 mr-2 mb-2 dark:bg-green-700 dark:text-white dark:border-green-700 ">View Product</button>
    </div>
</div>
<div class="max-w-sm bg-white rounded-lg border border-gray-200 shadow-md dark:bg-gray-800 dark:border-gray-700">
    <a href="#">
        <img class="rounded-t-lg" src="../static/imgs/nassim-boughazi-dodzmVtjoKs-unsplash.jpg" alt="">
    </a>
    <div class="p-5 text-center">
        <a href="#">
            <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white">Nike Lebrown-18</h5>
        </a>
        <nuxt-link to="/details">
        <button type="button" class="text-green-700 bg-white border border-green-700 focus:outline-none hover:bg-green-700 focus:ring-4 focus:ring-gray-200 font-medium rounded-lg text-sm px-5 py-2.5 mr-2 mb-2 dark:bg-green-700 dark:text-white dark:border-green-700 ">View Product</button>
      </nuxt-link>
    </div>
</div>

 </div>
<div class="flex justify-center gap-5">
 <Cards
            v-for="n in [1,2,3,4]"
            :key="n"
            title="Apple Watch Series 7 GPS, Aluminium Case, Starlight Sport"
            details="Lorem ipsum dolor sit,adipisicing elit. Sequi rem nobis in eius! "
            :price="300"
            :tourImage="require('@/static/imgs/men.jpg')"
          />

        </div>
 <h1 class="text-4xl text-center  mt-20">New arrivals today </h1>
 <!-- <div class="text-center">
<img class="max-w-full h-auto" src="../static/imgs/freestocks-_3Q3tsJ01nc-unsplash-removebg-preview.png" alt="image description">
</div> -->

<section class="overflow-hidden text-gray-700">
  <div class="container px-5 py-2 mx-auto lg:pt-24 lg:px-32">
    <div class="flex flex-wrap -m-1 md:-m-2">
      <div class="flex flex-wrap w-1/2">
        <div class="w-1/2 p-1 md:p-2">
          <img alt="gallery" class="block object-cover object-center w-full h-full rounded-lg"
            src="../static/imgs/tamara-bellis-CuXt1N5SjlE-unsplash.jpg">
        </div>
        <div class="w-1/2 p-1 md:p-2">
          <img alt="gallery" class="block object-cover object-center w-full h-full rounded-lg"
          src="../static/imgs/emily-pottiger-Zx76sbAndc0-unsplash (1).jpg">
        </div>
        <div class="w-full p-1 md:p-2">
          <img alt="gallery" class="block object-cover object-center w-full h-full rounded-lg"
          src="../static/imgs/pants.jpg">
        </div>
      </div>
      <div class="flex flex-wrap w-1/2">
        <div class="w-full p-1 md:p-2">
          <img alt="gallery" class="block object-cover object-center w-full h-full rounded-lg"
          src="../static/imgs/pp.jpg">
          </div>
        <div class="w-1/2 p-1 md:p-2">
          <img alt="gallery" class="block object-cover object-center w-full h-full rounded-lg"
            src="../static/imgs/tamara-bellis-Dv0YZ2_V3nc-unsplash.jpg">
        </div>
        <div class="w-1/2 p-1 md:p-2">
          <img alt="gallery" class="block object-cover object-center w-full h-full rounded-lg"
          src="../static/imgs/tobias-tullius-Fg15LdqpWrs-unsplash.jpg"> 
        </div>
      </div>
    </div>
  </div>
</section>

<div class="inline-flex justify-center items-center w-full">
    <hr class="my-8 w-64 h-1 bg-gray-200 rounded border-0 dark:bg-gray-700">
    <div class="absolute left-1/2 px-4 bg-white -translate-x-1/2 dark:bg-gray-900">
        <svg aria-hidden="true" class="w-5 h-5 text-gray-700 dark:text-gray-300" viewBox="0 0 24 27" fill="none" xmlns="http://www.w3.org/2000/svg"><path d="M14.017 18L14.017 10.609C14.017 4.905 17.748 1.039 23 0L23.995 2.151C21.563 3.068 20 5.789 20 8H24V18H14.017ZM0 18V10.609C0 4.905 3.748 1.038 9 0L9.996 2.151C7.563 3.068 6 5.789 6 8H9.983L9.983 18L0 18Z" fill="currentColor"></path></svg>
    </div>
</div>
</div>
 </template>   
   
