<template>
  <section class="relative py-20 2xl:py-40 bg-gray-800 overflow-hidden">
    <img
      class="hidden lg:block absolute top-0 right-0 h-128 w-128 -mt-52 -mr-52"
      src=""
      alt=""
    />
    <img
      class="hidden lg:block absolute bottom-0 left-0 h-128 w-128 -mb-52"
      src=""
      alt=""
    />
    <img
      class="block absolute bottom-0 left-0 h-24 md:h-32 lg:h-72 lg:ml-24 -mb-8"
      src=""
      alt=""
    />
    <img
      class="block absolute bottom-0 left-0 h-128 w-128 -mb-96 -ml-24"
      src=""
      alt=""
    />
    <div id="getstarted" class="container px-3 mx-auto">
      <div class="max-w-3xl mx-auto text-center">
        <h2 class="my-10 text-5xl lg:text-6xl font-bold font-heading text-white"
          >Refer a client to us if they signup you get free service for a month
          .</h2
        >
        <div class="max-w-md mx-auto">
          <p class="mb-20 text-lg text-gray-200"
            >all you have to do is give us their email address.</p
          >
          <a
            class="inline-block transition ease-in-out delay-150 hover:-translate-y-1 border-2 hover:scale-110 mb-4 sm:mb-0 sm:mr-4 py-5 px-12 text-white font-bold bg-gradient-to-r from-green-300 via-yellow-300 to-pink-300 hover:bg-blue-600 rounded-full duration-200"
            href="#porto"
            >Refer a client</a
          ><a
            class="inline-block transition ease-in-out delay-150 hover:-translate-y-1 hover:scale-110 hover:bg-indigo-500 py-5 px-12 text-white font-bold border border-gray-300 hover:border-gray-200 rounded-full"
            href="#how"
            >How it works</a
          >
        </div>
      </div>
    </div>
  </section>
  <div id="porto" class="bg-gray-800 py-6 sm:py-8 lg:py-12">
    <div class="max-w-screen-2xl px-4 md:px-8 mx-auto">
      <div
        class="md:h-80 flex flex-col sm:flex-row bg-gray-900 rounded-lg overflow-hidden"
      >
        <!-- content - start -->
        <div class="w-full sm:w-1/2 lg:w-2/5 flex flex-col p-4 sm:p-8">
          <h2 class="text-white text-xl md:text-2xl lg:text-4xl font-bold mb-4"
            >Get free service <br />for a month.</h2
          >

          <p class="max-w-md text-gray-400 mb-8"
            >We just trying to find ways to give you free data refer a client
            to us if they signup you get free service for a month .</p
          >

          <div class="mt-auto">
            <a
              href="#"
              class="inline-block transition ease-in-out delay-150 hover:-translate-y-1 border-2 hover:scale-110 mb-4 sm:mb-0 sm:mr-4 py-5 px-12 text-white font-bold bg-gradient-to-r from-green-300 via-yellow-300 to-pink-300 hover:bg-blue-600 rounded-full duration-200"
              >Learn More</a
            >
          </div>
        </div>
        <!-- content - end -->

        <!-- image - start -->
        <div
          class="w-full sm:w-1/2 lg:w-3/5 h-48 sm:h-auto order-first sm:order-none bg-gray-700 hover:scale-110 transition duration-300 ease-in-out"
        >
          <img
            src="https://images.unsplash.com/photo-1505846951821-e25bacf2eccd?auto=format&q=75&fit=crop&crop=top&w=1000&h=500"
            loading="lazy"
            alt="Photo by Dom Hill"
            class="w-full h-full object-cover object-center"
          />
        </div>
        <!-- image - end -->
      </div>
    </div>
  </div>

  <section class="relative bg-gray-800 pt-20 2xl:pt-40" id="#relative">
    <div id="how" class="container px-4 mx-auto mb-16 md:mb-24">
      <div class="text-center">
        <a class="inline-block mb-8 text-2xl font-bold" href="#">
          <img class="h-7" src="" alt="" width="auto" />
        </a>
        <h2 class="mb-8 text-white text-6xl 2xl:text-7xl font-bold font-heading"
          >Simple process.</h2
        >
        <p class="mb-16 text-xl text-white"
          >we only need the email address will do the rest</p
        >
        <a
          class="inline-block transition ease-in-out delay-150 hover:-translate-y-1 border-2 hover:scale-110 mb-4 sm:mb-0 sm:mr-4 py-5 px-12 text-white font-bold bg-gradient-to-r from-green-300 via-yellow-300 to-pink-300 hover:bg-blue-600 rounded-full duration-200"
          href="#"
          >Click here</a
        >
      </div>
    </div>
    <div class="relative">
      <img
        class="lg:relative lg:max-w-4xl mx-auto"
        src="zospace-assets/images/smartphone.png"
        alt=""
      />
    </div>
  </section>

  <div class="bg-gray-800">
    <div class="max-w-screen-xl mx-auto py-12 px-4 sm:px-6 lg:py-16 lg:px-8">
      <h2
        class="text-3xl leading-9 font-extrabold tracking-tight text-white sm:text-4xl sm:leading-10"
      >
        key in the clients email address
        <br class="hidden sm:inline" />
        <span class="text-white-600 text-lg">Refer a client to Afrihost</span>
      </h2>
      <form @submit="submitHandler" class="mt-8 sm:flex">
        <input
          aria-label="Email address"
          type="email"
          required
          class="appearance-none w-full px-5 py-3 border border-gray-300 text-base leading-6 rounded-md text-gray-900 bg-white placeholder-gray-500 focus:outline-none focus:shadow-outline focus:border-blue-300 transition duration-150 ease-in-out sm:max-w-xs"
          placeholder="clients email address"
        />
        <div class="mt-3 rounded-md shadow sm:mt-0 sm:ml-3 sm:flex-shrink-0">
          <button
            class="w-full flex items-center justify-center px-5 py-3 border border-transparent text-base leading-6 font-medium rounded-md text-white bg-gradient-to-r from-green-300 via-yellow-300 to-pink-300 hover:bg-indigo-500 focus:outline-none focus:shadow-outline transition duration-150 ease-in-out"
          >
            Submit email
          </button>
        </div>
      </form>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      takenNamePartials: ["faith", "ejiro", "sam", "josh"],
    };
  },
  methods: {
    submitHandler() {
      alert("Thank you for submitting this !");
    },
    async checkUsername({ value }) {
      // check to see if the username contains any of
      // our partial matches to simulate taken usernames.
      // wrap it in a promise and timeout to simulate an xhr request.
      let match = false;
      await new Promise((resolve) => {
        setTimeout(() => {
          // use .find() to check for matches and bail on first success
          match = this.takenNamePartials.find((partial) =>
            value.includes(partial)
          );
          resolve();
        }, 2000);
      });
      // return the cooreced boolean value of !match
      return !match;
    },
  },
};
</script>
