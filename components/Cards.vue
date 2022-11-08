<template>
    <div>
        <div class=" flex justify-evenly mt-10">
   <div class="max-w-sm bg-white rounded-lg border border-gray-200 shadow-md dark:bg-gray-800 dark:border-gray-700">
    <a href="#">
        <div><img :src="tourImage" /></div>
        <!-- <img class="rounded-t-lg" src="../static/imgs/dom-hill-nimElTcTNyY-unsplash.jpg" alt=""> -->
    </a>
    <div class="p-5 text-center">
        <a href="#">
            <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white">{{title}}</h5>
        </a>
        <button type="button" class="text-green-700 bg-white border border-green-700 focus:outline-none hover:bg-green-700 focus:ring-4 focus:ring-gray-200 font-medium rounded-lg text-sm px-5 py-2.5 mr-2 mb-2 dark:bg-green-700 dark:text-white dark:border-green-700 ">View Product</button>
    </div>
</div>
</div>  
    </div>
</template>
<script>
export default{
    props: {
    tourImage: {
      type: String,
      required: true,
    },
    title: {
      type: String,
      default: ""
    },
    details: {
      type: String,
      required: true,
    },
    price: {
      type: Number,
      required: true,
    },
  },
} 
</script>