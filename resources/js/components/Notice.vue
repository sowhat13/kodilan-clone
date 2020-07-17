<template>
  <div class="border-b border-gray-400 grid grid-cols-6 gap-4 py-2 px-1">
    <div class="col-span-1 flex items-center">
    <img :src="image" />
    </div>
    <div class="col-span-4">
      <div class="mt-1">
        <p class="text-lg font-hairline text-gray-800">{{title}}</p>
      </div>
      <div class="mt-6 flex items-center">
        <i class="fas fa-briefcase text-sm text-gray-500"></i>
        <p class="mx-1 text-sm text-green-500">{{company}}</p>

        <div class="mx-2 flex items-center">
          <i class="far fa-map text-sm text-gray-500"></i>
          <p class="text-sm text-green-500 font-thin mx-1">{{location}}</p>
        </div>
      </div>
      <div class="flex flex-wrap mt-2">
        <span class="border border-gray-400 text-green-500 px-1 text-xs rounded-sm m-1">linux</span>
      </div>
    </div>
    <div class="col-span-1 mt-1">
      <div class="flex flex-col">
        <span
          class="mx-auto border-2 border-blue-400 text-blue-600 rounded py-1 px-2 text-xs"
        >{{workingType}}</span>
        <span class="mx-auto text-xs text-gray-600 mt-1">{{publishedAt}}</span>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  props: ["title", "workingType", "image", "company", "location", "publishedAt"]
};
</script>

<style>
</style>
