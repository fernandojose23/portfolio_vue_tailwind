<template>
  <div>
    <section id="navbar">
      <header class="absolute top-0 left-0 w-full bg-transparent">
        <nav
          class="container max-w-6xl mx-auto flex justify-between items-center px-10 py-5 lg:px-10"
        >
          <div class="flex">
            <p class="text-sm font-semibold text-gray-100">FernandoJose. (Not Mobile Responsible)(59% in-progress)</p>
          </div>
          <div
            class="z-10 lg:flex items-center space-x-4 font-normal border border-gray-300 dark:border-gray-700 text-gray-100 bg-transparent backdrop-blur-lg text-sm pr-2 pl-10 py-2 rounded-full shadow-sm"
          >
            <a href="#home"><button>Home</button></a>
            <a href="#projects"><button>Projects</button></a>
            <a href="#skills"><button>Skills</button></a>
            <button
              class="border rounded-full p-2 hover:bg-gray-800 duration-500 hover:shadow-lg dark:bg-yellow-400"
              @click="toggleDarkMode"
            >
              <svg
                class="w-[20px] h-[20px] text-gray-100 dark:text-gray-900"
                aria-hidden="true"
                xmlns="http://www.w3.org/2000/svg"
                width="24"
                height="24"
                fill="none"
                viewBox="0 0 24 24"
              >
                <path
                  v-if="!darkMode"
                  stroke="currentColor"
                  stroke-linecap="round"
                  stroke-linejoin="round"
                  stroke-width="1.3"
                  d="M12 21a9 9 0 0 1-.5-17.986V3c-.354.966-.5 1.911-.5 3a9 9 0 0 0 9 9c.239 0 .254.018.488 0A9.004 9.004 0 0 1 12 21Z"
                />
                <path
                  v-else
                  stroke="currentColor"
                  stroke-linecap="round"
                  stroke-linejoin="round"
                  stroke-width="1.3"
                  d="M12 5V3m0 18v-2M7.05 7.05 5.636 5.636m12.728 12.728L16.95 16.95M5 12H3m18 0h-2M7.05 16.95l-1.414 1.414M18.364 5.636 16.95 7.05M16 12a4 4 0 1 1-8 0 4 4 0 0 1 8 0Z"
                />
              </svg>
            </button>
          </div>
        </nav>
      </header>
    </section>
  </div>
</template>

<script>
export default {
  data() {
    return {
      darkMode: localStorage.getItem("darkMode") === "true",
    };
  },
  mounted() {
    // Apply dark mode on initial load based on local storage
    document.documentElement.classList.toggle("dark", this.darkMode);
  },
  methods: {
    toggleDarkMode() {
      this.darkMode = !this.darkMode;
      // Store preference in local storage
      localStorage.setItem("darkMode", this.darkMode);
      document.documentElement.classList.toggle("dark", this.darkMode);
    },
  },
};
</script>

<style lang="scss" scoped></style>
