<template>
  <div id="navbar" class="block bg-white">
    <a href="#default" id="logo" class="px-3 py-2 ml-12">
      <span class="flex items-center">
        <span class="text-green-600 text-5xl">{</span>
        <span class="font-light ml-1 text-4xl">kod</span>
        <span class="text-3xl text-green-600 mr-1">,</span>
        <span class="mr-1 text-4xl">ilan</span>
        <span class="text-green-600 text-5xl">}</span>
      </span>
    </a>
    <div id="navbar-right" class="mr-12">
      <a class="bg-gray-700 border border-gray-500 text-white mx-3 px-5 py-2">
        <i class="fas fa-bullhorn"></i> Abone Ol
      </a>
      <a class="bg-green-600 text-white mx-3 px-5 py-2">Ücretsiz İlan Ekle</a>
    </div>
  </div>
</template>

<script>
export default {};

window.onscroll = function() {
  scrollFunction();
};

const scrollFunction = () => {
  if (document.body.scrollTop > 50 || document.documentElement.scrollTop > 50) {
    document.getElementById("navbar").style.padding = "20px 10px";
    document.getElementById("logo").style.fontSize = "25px";
  } else {
    document.getElementById("navbar").style.padding = "30px 10px";
    document.getElementById("logo").style.fontSize = "35px";
  }
};
</script>

<style scoped>
#navbar {
  overflow: hidden;
  padding: 40px 10px;
  transition: 1s;
  position: fixed;
  width: 100%;
  top: 0;
}

#navbar a {
  float: left;
  text-align: center;
  text-decoration: none;
  line-height: 25px;
  border-radius: 4px;
}

#navbar #logo {
  transition: 0.4s;
}

#navbar-right {
  float: right;
}

@media screen and (max-width: 580px) {
  #navbar {
    padding: 20px 10px !important;
  }
  #navbar a {
    float: none;
    display: block;
    text-align: left;
    margin: 15px 5px;
  }
  #navbar-right {
    float: none;
  }
}
</style>
