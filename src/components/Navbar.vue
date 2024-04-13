<template>
  <div>
    <section id="navbar">
      <header class="z-20 fixed sm:absolute top-0 left-0 w-full bg-transparent">
        <nav
          class="container max-w-6xl mx-auto flex justify-between items-center px-10 py-5 lg:px-10"
        >
          <div class="flex">
            <p class="hidden sm:block text-sm font-semibold text-neutral-100">
              FernandoJose.
            </p>
          </div>
          <div
            class="justify-between w-full sm:w-auto z-10 flex flex-wrap sm:flex-nowrap items-center space-x-4 font-normal border-2 border-neutral-300 dark:border-gray-700 text-gray-100 bg-transparent backdrop-blur-lg text-sm pr-2 pl-10 py-2 rounded-full shadow-sm"
          >
            <a href="#home"
              ><button class="flex flex-row items-center">
                <span
                  ><svg
                    class="w-6 h-6 me-2 block sm:hidden text-neutral-700 dark:text-gray-100"
                    aria-hidden="true"
                    xmlns="http://www.w3.org/2000/svg"
                    width="24"
                    height="24"
                    fill="none"
                    viewBox="0 0 24 24"
                  >
                    <path
                      stroke="currentColor"
                      stroke-linecap="round"
                      stroke-linejoin="round"
                      stroke-width="1"
                      d="m4 12 8-8 8 8M6 10.5V19a1 1 0 0 0 1 1h3v-3a1 1 0 0 1 1-1h2a1 1 0 0 1 1 1v3h3a1 1 0 0 0 1-1v-8.5"
                    />
                  </svg> </span
                ><span class="hidden sm:block"> Home </span>
              </button></a
            >
            <a href="#projects"
              ><button class="flex flex-row items-center">
                <span>
                  <svg
                    class="w-6 h-6 me-2 block sm:hidden text-neutral-700 dark:text-gray-100"
                    aria-hidden="true"
                    xmlns="http://www.w3.org/2000/svg"
                    width="24"
                    height="24"
                    fill="none"
                    viewBox="0 0 24 24"
                  >
                    <path
                      stroke="currentColor"
                      stroke-linecap="round"
                      stroke-linejoin="round"
                      stroke-width="1"
                      d="m10.051 8.102-3.778.322-1.994 1.994a.94.94 0 0 0 .533 1.6l2.698.316m8.39 1.617-.322 3.78-1.994 1.994a.94.94 0 0 1-1.595-.533l-.4-2.652m8.166-11.174a1.366 1.366 0 0 0-1.12-1.12c-1.616-.279-4.906-.623-6.38.853-1.671 1.672-5.211 8.015-6.31 10.023a.932.932 0 0 0 .162 1.111l.828.835.833.832a.932.932 0 0 0 1.111.163c2.008-1.102 8.35-4.642 10.021-6.312 1.475-1.478 1.133-4.77.855-6.385Zm-2.961 3.722a1.88 1.88 0 1 1-3.76 0 1.88 1.88 0 0 1 3.76 0Z"
                    />
                  </svg> </span
                ><span class="hidden sm:block"> Projects </span>
              </button></a
            >
            <a href="#skills"
              ><button class="flex flex-row items-center">
                <span>
                  <svg
                    class="w-6 h-6 me-2 block sm:hidden text-neutral-700 dark:text-gray-100"
                    aria-hidden="true"
                    xmlns="http://www.w3.org/2000/svg"
                    width="24"
                    height="24"
                    fill="none"
                    viewBox="0 0 24 24"
                  >
                    <path
                      stroke="currentColor"
                      stroke-linecap="round"
                      stroke-linejoin="round"
                      stroke-width="1"
                      d="m8 8-4 4 4 4m8 0 4-4-4-4m-2-3-4 14"
                    />
                  </svg> </span
                ><span class="hidden sm:block"> Skills </span>
              </button></a
            >
            <button
              class="border-2 rounded-full p-2 hover:bg-gray-800 bg-gray-700 duration-500 hover:shadow-lg dark:bg-yellow-400"
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
