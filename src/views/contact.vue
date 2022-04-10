<template>
  <div class="home">
    <contactpage msg="Welcome to Your Vue.js App" />
    <footerpage msg="Welcome to Your Vue.js App" />
  </div>
</template>

<script>
// @ is an alias to /src
import contactpage from "@/components/contactpage.vue";
import footerpage from "@/components/footerpage.vue";

export default {
  name: "contact",
  components: {
    contactpage,
    footerpage,
  },
};
</script>
