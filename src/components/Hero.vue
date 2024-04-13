<template>
  <section id="home">
    <div
      class="max-w-7xl container px-5 h-screen mx-auto flex items-center justify-center"
    >
      <div class="lg:w-4/6">
        <div class="flex flex-col sm:flex-row">
          <div class="sm:p-8 p-8 mt-4 pt-4 sm:mt-0">
            <div class="flex flex-col gap-2">
              <p class="text-lg font-medium text-neutral-200">Hi, My Name is</p>
              <p class="text-3xl sm:text-5xl font-semibold text-neutral-100">
                Fernando Jose A. Lopez
              </p>
              <p class="text-base font-normal text-neutral-200 mt-2">
                CLSU BSIT graduate with a focus on system development. Skilled
                in front-end and back-end web development. Proficient in
                creating user-friendly and dynamic web applications using
                various programming languages, frameworks, and tools.
              </p>
            </div>
            <div class="flex flex-col sm:flex-row mt-4">
              <button
                type="button"
                class="sm:w-auto w-full z-10 inline-flex items-center text-center justify-center duration-500 hover:scale-105 hover:shadow-xl cursor-pointer text-white bg-blue-500 hover:bg-blue-600 font-medium rounded-full text-sm px-5 py-2.5 me-2 mb-2 dark:bg-blue-600 dark:hover:bg-blue-700"
              >
                View Resume
                <svg
                  class="rtl:rotate-180 w-3.5 h-3.5 ms-2"
                  aria-hidden="true"
                  xmlns="http://www.w3.org/2000/svg"
                  fill="none"
                  viewBox="0 0 14 10"
                >
                  <path
                    stroke="currentColor"
                    stroke-linecap="round"
                    stroke-linejoin="round"
                    stroke-width="2"
                    d="M1 5h12m0 0L9 1m4 4L9 9"
                  ></path>
                </svg>
              </button>
              <a href="#contact" class="z-10">
                <button
                  type="button"
                  class="w-full text-gray-900 bg-white border duration-500 hover:scale-105 hover:shadow-xl cursor-pointer border-gray-300 hover:bg-gray-100 font-medium rounded-full text-sm px-5 py-2.5 me-2 mb-2 dark:bg-gray-800 dark:text-white dark:border-gray-600 dark:hover:bg-gray-700 dark:hover:border-gray-600 dark:focus:ring-gray-700"
                >
                  Contact me
                </button>
              </a>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script setup></script>

<style lang="scss" scoped></style>
