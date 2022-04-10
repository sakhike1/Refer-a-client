<template>
  <div class="footer">
    <footerpage msg="Welcome to Your Vue.js App" />
  </div>
</template>

<script>
// @ is an alias to /src
import footerpage from "@/components/footerpage.vue";

export default {
  name: "footer",
  components: {
    footerpage,
  },
};
</script>
