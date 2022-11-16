<template> 
<div>
   <Herosection/>
<div class="bgimage">
   <h1 class="text-red-700 text-center mt-20 text-4xl">New Arrivals Today</h1> 
    <div class="h-screen flex items-center justify-center">
      <form class="w-full md:w-1/3 bg-white rounded-lg items-center">
            <h2 class="text-3xl text-center text-gray-700 mb-4">Add New Products</h2>   
<div class="flex font-bold justify-center mt-6">
    <!-- <svg class="absolute -mt-20  w-14 h-14 text-center text-gray-400" fill="currentColor" viewBox="0 0 20 20" xmlns="http://www.w3.org/2000/svg"><path fill-rule="evenodd" d="M10 9a3 3 0 100-6 3 3 0 000 6zm-7 9a7 7 0 1114 0H3z" clip-rule="evenodd"></path></svg> -->
   <!-- <img class="h-24 w-24"
      src="./Images/avatar1.png"> -->
</div>

<div class="px-12 pb-10">
<div class="w-full mb-2">
   <div class="flex justify-center">
      <input type='text' v-model="title" placeholder="title"
         class="px-8  w-full border rounded py-2 text-gray-700 focus:outline-none items-center" />
   </div>
</div>

<div class="w-full mb-2">
   <div class="flex justify-center mb-2">
      <input type='text' v-model="description" placeholder="description"
         class="px-8  w-full border rounded py-2 text-gray-700 focus:outline-none items-center" />
   </div>

   <div class="w-full mb-2">
   <div class="flex justify-center mb-2">
      <input type='text' v-model="price" placeholder="price"
         class="px-8  w-full border rounded py-2 text-gray-700 focus:outline-none items-center" />
   </div>
</div>
</div>

<label class="block mb-2 text-sm font-medium text-gray-900 dark:text-gray-300" for="user_avatar">Upload file</label>
<input type="file"   placeholder="image"
class="block w-full text-sm text-gray-900 bg-gray-50 rounded-lg border border-gray-300 cursor-pointer dark:text-gray-400 focus:outline-none dark:bg-gray-700 dark:border-gray-600 dark:placeholder-gray-400" aria-describedby="user_avatar_help">
</div>
<button type="button" @click="addproducts"
   class="w-full mt-6 py-2  rounded bg-blue-500 text-gray-100  focus:outline-none ">Add Product</button>
   <!-- <NuxtLink to="/" class="text-center">
  <button type="button" class="text-green-700 text-2xl bg-white border uppercase border-green-700 focus:outline-none hover:bg-green-700 hover:text-white focus:ring-4 focus:ring-gray-200 font-medium rounded-lg  px-5 py-2.5 mr-2 mb-2 dark:bg-green-700 dark:text-white dark:border-green-700 ">logout</button>
</NuxtLink> -->
        </form>

        
    </div>
  
    <Ads/>
</div>
</div>
</template>
<script>
const axios = require("axios");
const sweetalert = require("sweetalert");
export default{
    data(){
      return{
         title:"",
         description:"",
         price:"",
         imageUrl:""
      };
   },
   methods:{
      addproducts(){
         console.log(this.title, this.description, this.price, this.imageUrl)
         const newCategory={
            title : this.title,
            description : this.description,
            price:this.price,
            imageUrl: this.imageUrl
         };
         const baseURL="http://localhost:8070/api/all-products";
         url:`${baseURL}/products/add`
         axios({
            method : 'post',
            data:JSON.stringify(newCategory),
            Headers:{
               'Content-Type': 'application/json'
            }
         })
         .then(()=>{
            sweetalert({
               text:"product added sucessfully",
               icon:"sucess"
            })
         })
         .catch((err)=>{
            console.log(err);
         });
      }
   },
   mounted(){
  }
   
} 
</script>
<style scoped>
.bgimage{
   background-image: url(../static/imgs/alex-haigh-fEt6Wd4t4j0-unsplash.jpg);
}
</style>