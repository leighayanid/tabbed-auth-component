<template>
 <div class="flex flex-row w-full">
    <div class="bg flex h-50 w-full bg-cover"></div>
    <div class="flex flex-col h-full w-full">
      <div class="p-10">
        <div class="text-black font-bold text-xl text-center mb-5">
          Register
        </div>
        <div class="form-register">
          <div class="flex flex-col justify-center">
            <input type="text" placeholder="Full Name" class="shadow-md py-2 px-5 mb-5 rounded italic">
            <input type="text" placeholder="Email address" class="shadow-md py-2 px-5 mb-5 rounded italic">
            <input type="password" placeholder="Password" class="shadow-md py-2 px-5 mb-5 rounded italic">
            <input type="password" placeholder="Confirm Password" class="shadow-md py-2 px-5 mb-5 rounded italic">
            <div class="flex flex-row justify-center mb-5">
              <input type="checkbox" class="shadow-md py-2 px-5 rounded">
              <label for="" class="text-sm text-gray-700 ml-2">I have read the terms and agreement.</label>
            </div>
            <button class="bg-red-700 text-white rounded p-2 hover:bg-gray-500 hover:text-red-700 hover:shadow-lg">
              Register
            </button>
          </div>
      </div>
    </div>
    </div>
  </div>
</template>
<style scoped>
  .bg{
    background: url(~assets/img/bg2.jpg);
    background-size: cover;
    background-position: center;
    background-repeat: no-repeat;
  }
</style>