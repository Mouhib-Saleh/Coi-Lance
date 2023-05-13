<template>
   
<header class="bg-white shadow">
        <div class="max-w-7xl mx-auto py-6 px-4 sm:px-6 lg:px-8">
          <h1 class="text-3xl font-bold leading-tight text-gray-900">
            Products
          </h1>
        </div>
      </header>
      <main>

        <div class="max-w-7xl mx-auto py-6 sm:px-6 lg:px-8">
          <div class="px-4 py-6 sm:px-0">

            <div class="flex flex-col md:flex-row mb-4">
                <div class="w-full md:w-1/4 lg:w-1/4 bg-gray-300">
                    <div style="padding: 2rem;"> 
                <p ></p>
                    </div>
                </div>
                <div class="w-full md:w-3/4 lg:w-3/4 " >
                    <div style="display: flex;align-items: center;justify-content: center;">
                            <form class="flex items-center" style="width: 88%;margin-top: 10px;">   
                                <label for="simple-search" class="sr-only">Search</label>
                                <div class="relative w-full">
                                    <div class="absolute inset-y-0 left-0 flex items-center pl-3 pointer-events-none">
                                        <svg aria-hidden="true" class="w-5 h-5 text-gray-500 " fill="currentColor" viewBox="0 0 20 20" xmlns="http://www.w3.org/2000/svg"><path fill-rule="evenodd" d="M8 4a4 4 0 100 8 4 4 0 000-8zM2 8a6 6 0 1110.89 3.476l4.817 4.817a1 1 0 01-1.414 1.414l-4.816-4.816A6 6 0 012 8z" clip-rule="evenodd"></path></svg>
                                    </div>
                                    <input type="text" id="simple-search" class="bg-gray-50 border border-gray-300 text-gray-900 text-sm rounded-lg focus:ring-teal-500 focus:border-teal-500 block w-full pl-10 p-2.5 " placeholder="Search" required>
                                </div>
                                <button type="submit" class="p-2.5 ml-2 text-sm font-medium text-white bg-teal-700 rounded-lg border border-teal-700 hover:bg-teal-800 focus:ring-4 focus:outline-none focus:ring-teal-300 ">
                                    <svg class="w-5 h-5" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M21 21l-6-6m2-5a7 7 0 11-14 0 7 7 0 0114 0z"></path></svg>
                                    <span class="sr-only">Search</span>
                                </button>
                            </form>
                    </div>
                    <div class="per" >
                    <ProductCard :product="product"/>
                    <ProductCard :product="product"/>
                    </div>
                </div>
            </div> 
          </div>
        </div>
      </main>
    
</template>

<script setup>
    const product = {
         name: "Beer",
         price: 2.99,
         description: "This is a beer"
    }
</script>

<style  scoped>
.per{
    display: flex;
    flex-direction: col;
    justify-content: center;
    flex-wrap: wrap;
    flex: 1;
    gap: 1rem;
    padding: 1rem;
}

</style>