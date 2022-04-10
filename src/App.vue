<template class="bg-gradient-to-r from-pink-500 via-red-500 to-yellow-500">
  <div id="nav">
    <nav
      class="bg-gradient-to-r from-green-300 via-yellow-300 to-pink-300 border-gray-200 px-2 sm:px-4 py-2.5 rounded dark:bg-gray-800"
    >
      <div
        class="container flex flex-wrap justify-between items-center mx-auto"
      >
        <a href="https://flowbite.com" class="flex items-center">
          <span
            class="self-center text-white ml-20 text-3xl font-semibold whitespace-nowrap dark:text-white"
            >Afrihost</span
          >
        </a>
        <div class="flex md:order-2">
          <router-link to="/contact/#how">
            <button
              type="button"
              class="rounded-3xl transition ease-in-out delay-150 hover:-translate-y-1 border-2 hover:scale-110 hover:bg-indigo-500 text-white bg-gradient-to-r from-green-300 via-blue-500 to-purple-600 focus:ring-4 focus:outline-none focus:ring-blue-300 font-medium text-sm px-5 py-2.5 text-center mr-3 md:mr-0 dark:bg-blue-600 dark:hover:bg-blue-700 dark:focus:ring-blue-800"
              >Get started</button
            >
          </router-link>
        </div>
        <div
          class="hidden justify-between items-center w-full md:flex md:w-auto md:order-1"
          id="mobile-menu-4"
        >
        </div>
      </div>
    </nav>
  </div>
  <router-view />
  <a @click="scrollTop" v-show="visible" class="bottom-right">
    <slot></slot>
  </a>
</template>

<script>
import { ref } from "vue";

export default {
  setup() {},
  methods: {
    goTo(getstarted) {
      this.$router.push("/getstarted");
    },
  },
};
</script>

<style lang="css">
@import url("https://fonts.googleapis.com/css2?family=Poppins:wght@200;300;400;500;600;700&display=swap");
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: "Poppins", sans-serif;
}
body {
  background-color: linear-gradient(
    #051937,
    #004d7a,
    #008793,
    #00bf72,
    #a8eb12
  );
}
nav {
  display: flex;
  height: 80px;
  width: 100%;
  background: #ffffff;
  align-items: center;
  justify-content: space-between;
  padding: 0 50px 0 100px;
  flex-wrap: wrap;
}
nav .logo {
  color: rgb(180, 173, 173);
  font-size: 20px;
  font-weight: 400;
}
nav ul {
  display: flex;
  flex-wrap: wrap;
  list-style: none;
}
nav ul li {
  margin: 0 5px;
}
nav ul li a {
  color: #000000;
  text-decoration: none;
  font-size: 14px;
  font-weight: 500;
  padding: 8px 15px;
  border-radius: 5px;
  letter-spacing: 1px;
  transition: all 0.3s ease;
}
nav ul li a.active,
nav ul li a:hover {
  color: #111;
  border-radius: 5px;
  background: #ffffff;
  align-items: center;
  justify-content: space-between;
  flex-wrap: wrap;
  padding: 8px 15px;
}
nav .menu-btn i {
  color: rgb(0, 0, 0);
  font-size: 22px;
  cursor: pointer;
  display: none;
}
input[type="checkbox"] {
  display: none;
}
@media (max-width: 1000px) {
  nav {
    padding: 0 40px 0 50px;
  }
}
@media (max-width: 920px) {
  nav .menu-btn i {
    display: block;
  }
  #click:checked ~ .menu-btn i:before {
    content: "\f00d";
  }
  nav ul {
    position: absolute;
    top: 80px;
    left: -100%;
    background: #ecd2d2;
    height: 70vh;
    width: 100%;
    text-align: center;
    display: block;
    transition: all 0.3s ease;
    z-index: 100;
  }
  #click:checked ~ ul {
    left: 0;
  }
  nav ul li {
    width: 100%;
    margin: 40px 0;
  }
  nav ul li a {
    width: 100%;
    margin-left: -100%;
    display: block;
    font-size: 13px;
    transition: 0.6s cubic-bezier(0.68, -0.55, 0.265, 1.55);
  }
  #click:checked ~ ul li a {
    margin-left: 0px;
  }
  nav ul li a.active,
  nav ul li a:hover {
    background: none;
    color: rgb(16, 216, 9);
  }
}
.content {
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  text-align: center;
  z-index: -1;
  width: 100%;
  padding: 0 30px;
  color: #1b1b1b;
}
.content div {
  font-size: 40px;
  font-weight: 700;
}
</style>
