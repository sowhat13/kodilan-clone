<template>
  <div class="bg-gray-800 mt-32">
    <div class="py-16 px-20">
      <div>
        <h1 class="ml-4 mb-10 text-white text-4xl">İlan Ara</h1>
        <div class="lg:flex">
          <input
            class="shadow appearance-none border rounded my-4 lg:my-0 lg:mx-4 w-full py-4 px-4 text-gray-700 leading-tight focus:outline-none focus:shadow-outline"
            id="username"
            type="text"
            placeholder="Pozisyon adı, teknoloji adı"
          />
          <select
            class="appearance-none border bg-white rounded my-4 lg:my-0 lg:mx-4 w-full py-4 px-4 text-gray-700 leading-tight focus:outline-none focus:shadow-outline"
          >
            <option value disabled selected>Şehir seçiniz...</option>
            <option>Ankara</option>
            <option>Antalya</option>
            <option>Kayseri</option>
          </select>
          <div class="flex">
            <button class="mx-auto py-3 bg-green-500 text-white lg:px-8 block px-16 rounded">
              <i class="fas fa-search text-xl"></i>
            </button>
          </div>
        </div>
        <div class="lg:w-2/5 mt-4">
          <div class="ml-3 mt-1 flex flex-wrap">
            <span
              class="py-1 px-3 text-gray-400 rounded bg-transparent border border-gray-200 m-1"
            >Frontend</span>
            <span
              class="py-1 px-3 text-gray-400 rounded bg-transparent border border-gray-200 m-1"
            >Backend</span>
            <span
              class="py-1 px-3 text-gray-400 rounded bg-transparent border border-gray-200 m-1"
            >Mobile</span>
            <span
              class="py-1 px-3 text-gray-400 rounded bg-transparent border border-gray-200 m-1"
            >Devops</span>
            <span
              class="py-1 px-3 text-gray-400 rounded bg-transparent border border-gray-200 m-1"
            >İstanbul</span>
            <span
              class="py-1 px-3 text-gray-400 rounded bg-transparent border border-gray-200 m-1"
            >Ankara</span>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style scoped>
</style>