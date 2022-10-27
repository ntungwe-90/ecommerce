<template> 
<div>
    
    <div class="h-screen flex items-center justify-center">
       <form class="w-full md:w-1/3 bg-white rounded-lg items-center">
            <h2 class="text-3xl text-center text-gray-700 mb-4">Add New Products</h2>   
<div class="flex font-bold justify-center mt-6">
    <svg class="absolute -mt-20  w-14 h-14 text-center text-gray-400" fill="currentColor" viewBox="0 0 20 20" xmlns="http://www.w3.org/2000/svg"><path fill-rule="evenodd" d="M10 9a3 3 0 100-6 3 3 0 000 6zm-7 9a7 7 0 1114 0H3z" clip-rule="evenodd"></path></svg>
   <!-- <img class="h-24 w-24"
      src="./Images/avatar1.png"> -->
</div>

<div class="px-12 pb-10">
<div class="w-full mb-2">
   <div class="flex justify-center">
      <input type='text' placeholder="title"
         class="px-8  w-full border rounded py-2 text-gray-700 focus:outline-none items-center" />
   </div>
</div>

<div class="w-full mb-2">
   <div class="flex justify-center mb-2">
      <input type='text' placeholder="description"
         class="px-8  w-full border rounded py-2 text-gray-700 focus:outline-none items-center" />
   </div>

   <div class="w-full mb-2">
   <div class="flex justify-center mb-2">
      <input type='text' placeholder="price"
         class="px-8  w-full border rounded py-2 text-gray-700 focus:outline-none items-center" />
   </div>
</div>
</div>

<label class="block mb-2 text-sm font-medium text-gray-900 dark:text-gray-300" for="user_avatar">Upload file</label>
<input class="block w-full text-sm text-gray-900 bg-gray-50 rounded-lg border border-gray-300 cursor-pointer dark:text-gray-400 focus:outline-none dark:bg-gray-700 dark:border-gray-600 dark:placeholder-gray-400" aria-describedby="user_avatar_help" id="user_avatar" type="file">
</div>
<button type="submit"
   class="w-full mt-6 py-2  rounded bg-blue-500 text-gray-100  focus:outline-none ">Add Product</button>
        </form>
    </div>
<!-- <form>
  <div class="mb-6">
    <label for="email" class="block mb-2 text-sm font-medium text-gray-900 dark:text-gray-300">title</label>
    <input type="email" id="email" class="bg-gray-50 border border-gray-300 text-gray-900 text-sm rounded-lg focus:ring-blue-500 focus:border-blue-500 block w-full p-2.5 dark:bg-gray-700 dark:border-gray-600 dark:placeholder-gray-400 dark:text-white dark:focus:ring-blue-500 dark:focus:border-blue-500" placeholder="name@flowbite.com">
  </div>
  <div class="mb-6">
    <label for="password" class="block mb-2 text-sm font-medium text-gray-900 dark:text-gray-300">discription</label>
    <input type="password" id="password" class="bg-gray-50 border border-gray-300 text-gray-900 text-sm rounded-lg focus:ring-blue-500 focus:border-blue-500 block w-full p-2.5 dark:bg-gray-700 dark:border-gray-600 dark:placeholder-gray-400 dark:text-white dark:focus:ring-blue-500 dark:focus:border-blue-500" >
  </div>
  <div class="flex items-start mb-6">
    <div class="flex items-center h-5">
      <input id="remember" type="checkbox" value="" class="w-4 h-4 bg-gray-50 rounded border border-gray-300 focus:ring-3 focus:ring-blue-300 dark:bg-gray-700 dark:border-gray-600 dark:focus:ring-blue-600 dark:ring-offset-gray-800" >
    </div>
    <label for="remember" class="ml-2 text-sm font-medium text-gray-900 dark:text-gray-300">Remember me</label>
  </div>
  
<label class="block mb-2 text-sm font-medium text-gray-900 dark:text-gray-300" for="user_avatar">Upload file</label>
<input class="block w-full text-sm text-gray-900 bg-gray-50 rounded-lg border border-gray-300 cursor-pointer dark:text-gray-400 focus:outline-none dark:bg-gray-700 dark:border-gray-600 dark:placeholder-gray-400" aria-describedby="user_avatar_help" id="user_avatar" type="file">

  <button type="submit" class="text-white bg-blue-700 hover:bg-blue-800 focus:ring-4 focus:outline-none focus:ring-blue-300 font-medium rounded-lg text-sm w-full sm:w-auto px-5 py-2.5 text-center dark:bg-blue-600 dark:hover:bg-blue-700 dark:focus:ring-blue-800">Add</button>
</form> -->
</div>
</template>