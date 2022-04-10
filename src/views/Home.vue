<template>
  <div class="home">
    <HelloWorld msg="Welcome to Your Vue.js App" />
    <footerpage msg="Welcome to Your Vue.js App" />
  </div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from "@/components/HelloWorld.vue";
import footerpage from "@/components/footerpage.vue";

export default {
  name: "Home",
  components: {
    HelloWorld,
    footerpage,
  },
};
</script>
