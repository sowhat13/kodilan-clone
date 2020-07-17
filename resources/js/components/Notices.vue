<template>
  <div class="mt-10 grid grid-cols-3 gap-4">
    <div class="col-span-2">
      <div class="ml-20">
        <div class="mb-6">
          <h1 class="text-xl font-thin text-gray-700">En son eklenen ilanlar</h1>
        </div>
        <div class="flex justify-between items-center">
          <div>
            <button
              class="border-none focus:outline-none mr-1 bg-green-500 font-semibold text-white px-5 py-2 rounded-tl-sm rounded-bl-sm text-sm"
            >Bugün</button>
            <button
              class="border-none focus:outline-none bg-gray-300 text-gray-600 font-semibold px-5 py-2 text-sm"
            >Bu hafta</button>
            <button
              class="border-none focus:outline-none ml-1 bg-gray-300 text-gray-600 font-semibold px-5 py-2 rounded-tr-sm rounded-br-sm text-sm"
            >Bu ay</button>
          </div>
          <div>
            <button
              class="border-none focus:outline-none ml-1 bg-green-500 font-semibold text-white px-5 py-2 rounded-sm"
            >
              <i class="fa fa-plus-circle"></i> Tüm ilanları gör
            </button>
          </div>
        </div>
        <div class="my-5 border border-gray-400 rounded-sm">
          <notice
            v-for="job in jobs"
            :key="job.title"
            :title="job.title"
            :image="job.image"
            :workingType="job.workingType"
            :company="job.company"
            :location="job.location"
            :publishedAt="job.publishedAt"
          ></notice>
        </div>
      </div>
    </div>
    <div class="col-span-1 border border-red-300">1</div>
  </div>
</template>

<script>
import Featured from "./Featured";
import Notice from "./Notice";

export default {
  components: { Featured, Notice },
  data() {
    return {
      jobs: [
        {
          title: "PHP Developer",
          image:
            "https://customer-service.xyz/wp-content/uploads/2019/12/hepsiburada-logo.jpg",
          workingType: "Stajyer",
          company: "Hepsiburada",
          location: "İstanbul",
          publishedAt: "6 saat önce",
          tags: ["php", "symfony", "mysql"]
        },
        {
          title: "Senior Java Developer",
          image:
            "https://seeklogo.com/images/Y/yemek-sepeti-logo-0961A3A1FD-seeklogo.com.png",
          workingType: "Tam zamanlı",
          company: "Yemek Sepeti",
          location: "İstanbul",
          publishedAt: "1 hafta önce",
          tags: ["java", "hibernate", "spring", "javafx", "android"]
        },
        {
          title: "iOS Developer",
          image:
            "https://patronlarinensesindeyiz.org/wp-content/uploads/2019/09/Copy-of-Copy-of-PEWeb-sa%C4%9Fda-filigranl%C4%B1-haber-fotosu-660x300-1-660x300.png",
          workingType: "Tam zamanlı",
          company: "Trendyol",
          location: "İstanbul",
          publishedAt: "1 gün önce",
          tags: ["swift", "objective-c", "mobile"]
        }
      ]
    };
  }
};
</script>
