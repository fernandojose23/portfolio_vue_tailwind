<template>
  <div class="scroll-smooth">
    <div class="area dark:bg-slate-900 duration-500">
      <Navbar></Navbar>
      <Hero></Hero>
      <ul class="circles blur-sm">
        <li></li>
        <li></li>
        <li></li>
        <li></li>
        <li></li>
        <li></li>
        <li></li>
        <li></li>
        <li></li>
        <li></li>
      </ul>
    </div>
    <Education></Education>
    <Experience></Experience>
    <Projects></Projects>
    <Skills></Skills>
    <Contact></Contact>
    <Footer></Footer>
    <a href="#navbar">
      <div
        class="fixed cursor-pointer hover:scale-110 shadow-md bg-transparent backdrop-blur-sm border dark:border-gray-700 duration-700 text-center p-0.5 leading-none rounded-full left-auto bottom-0 right-0 m-5"
      >
        <svg
          class="w-[45px] h-[43px] text-gray-700 dark:text-white duration-700"
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
            d="M12 6v13m0-13 4 4m-4-4-4 4"
          />
        </svg>
      </div>
    </a>
  </div>
</template>

<script setup>
import Navbar from "../components/Navbar.vue";
import Hero from "../components/Hero.vue";
import Education from "../components/Education.vue";
import Experience from "../components/Experience.vue";
import Projects from "../components/Projects.vue";
import Skills from "../components/Skills.vue";
import Contact from "../components/Contact.vue";
import Footer from "../components/Footer.vue";
// import ReviewPDF from "../components/ReviewPDF.vue";
</script>

<style></style>
