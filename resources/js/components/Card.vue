<template>
  <div class="bg-gray-800 mt-24">
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
            <badge v-for="tag in tags" :key="tag" :name="tag"></badge>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import Badge from "./Badge";

export default {
  components: {
    Badge
  },
  data() {
    return {
      tags: ["Ankara", "Frontend", "Backend", "Mobile", "İzmir", "Devops"]
    };
  }
};
</script>
