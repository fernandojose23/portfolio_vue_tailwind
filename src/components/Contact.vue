<template>
  <section id="contact" class="dark:bg-slate-900 duration-500">
    <div
      class="max-w-7xl container px-5 py-2 mx-auto flex items-center justify-center"
    >
      <div class="lg:w-4/6">
        <div class="flex flex-col sm:flex-row mt-10">
          <div class="sm:p-8 p-8 mt-4 pt-4 sm:mt-0">
            <div class="flex flex-col gap-2">
              <p class="text-2xl font-semibold dark:text-gray-100">
                Let's Connect 🤙
              </p>
              <p
                class="text-base font-normal text-gray-500 mt-2 dark:text-gray-400"
              >
                For web development collaborations, inquiries, or just to
                connect, don't hesitate to take the initiative and reach out via
                email. Whether it's discussing potential projects, sharing fan
                feedback, or simply having a casual chat, your message is always
                welcomed.
              </p>
            </div>
            <div class="mt-4">
              <form @submit.prevent="submitForm" class="space-y-8">
                <div>
                  <label
                    for="email"
                    class="block mb-2 text-sm font-medium text-gray-900 dark:text-gray-300"
                    >Your Email</label
                  >
                  <input
                    type="email"
                    id="email"
                    name="email"
                    v-model="formData.email"
                    class="shadow-sm bg-gray-50 border border-gray-300 text-gray-900 text-sm rounded-lg focus:ring-primary-500 focus:border-primary-500 block w-full p-2.5 dark:bg-gray-700 dark:border-gray-600 dark:placeholder-gray-400 dark:text-white dark:focus:ring-primary-500 dark:focus:border-primary-500 dark:shadow-sm-light"
                    placeholder="name@gmail.com"
                    required
                  />
                </div>
                <div>
                  <label
                    for="subject"
                    class="block mb-2 text-sm font-medium text-gray-900 dark:text-gray-300"
                    >Subject</label
                  >
                  <input
                    type="text"
                    id="subject"
                    name="subject"
                    v-model="formData.subject"
                    class="block p-3 w-full text-sm text-gray-900 bg-gray-50 rounded-lg border border-gray-300 shadow-sm focus:ring-primary-500 focus:border-primary-500 dark:bg-gray-700 dark:border-gray-600 dark:placeholder-gray-400 dark:text-white dark:focus:ring-primary-500 dark:focus:border-primary-500 dark:shadow-sm-light"
                    placeholder="Let us know how we can help you"
                    required
                  />
                </div>
                <div class="sm:col-span-2">
                  <label
                    for="message"
                    class="block mb-2 text-sm font-medium text-gray-900 dark:text-gray-400"
                    >Your Message</label
                  >
                  <textarea
                    id="message"
                    rows="6"
                    class="block p-2.5 w-full text-sm text-gray-900 bg-gray-50 rounded-lg shadow-sm border border-gray-300 focus:ring-primary-500 focus:border-primary-500 dark:bg-gray-700 dark:border-gray-600 dark:placeholder-gray-400 dark:text-white dark:focus:ring-primary-500 dark:focus:border-primary-500"
                    placeholder="Leave a message..."
                    name="message"
                    v-model="formData.message"
                  ></textarea>
                </div>
                <button
                  type="submit"
                  v-show="!isLoading"
                  class="duration-500 hover:scale-105 hover:shadow-xl cursor-pointer inline-flex items-center text-white bg-blue-500 hover:bg-blue-600 font-medium rounded-full text-sm px-5 py-2.5 text-center me-2 mb-2 dark:bg-blue-600 dark:hover:bg-blue-700"
                >
                  Send Message
                </button>
                <button
                  v-show="isLoading"
                  disabled
                  type="button"
                  class="hover:shadow-xl inline-flex items-center text-white bg-blue-500 hover:bg-blue-600 font-medium rounded-full text-sm px-5 py-2.5 text-center me-2 mb-2 dark:bg-blue-600 dark:hover:bg-blue-700"
                >
                  <svg
                    aria-hidden="true"
                    role="status"
                    class="inline w-4 h-4 me-3 text-neutral-100 animate-spin"
                    viewBox="0 0 100 101"
                    fill="none"
                    xmlns="http://www.w3.org/2000/svg"
                  >
                    <path
                      d="M100 50.5908C100 78.2051 77.6142 100.591 50 100.591C22.3858 100.591 0 78.2051 0 50.5908C0 22.9766 22.3858 0.59082 50 0.59082C77.6142 0.59082 100 22.9766 100 50.5908ZM9.08144 50.5908C9.08144 73.1895 27.4013 91.5094 50 91.5094C72.5987 91.5094 90.9186 73.1895 90.9186 50.5908C90.9186 27.9921 72.5987 9.67226 50 9.67226C27.4013 9.67226 9.08144 27.9921 9.08144 50.5908Z"
                      fill="#E5E7EB"
                    />
                    <path
                      d="M93.9676 39.0409C96.393 38.4038 97.8624 35.9116 97.0079 33.5539C95.2932 28.8227 92.871 24.3692 89.8167 20.348C85.8452 15.1192 80.8826 10.7238 75.2124 7.41289C69.5422 4.10194 63.2754 1.94025 56.7698 1.05124C51.7666 0.367541 46.6976 0.446843 41.7345 1.27873C39.2613 1.69328 37.813 4.19778 38.4501 6.62326C39.0873 9.04874 41.5694 10.4717 44.0505 10.1071C47.8511 9.54855 51.7191 9.52689 55.5402 10.0491C60.8642 10.7766 65.9928 12.5457 70.6331 15.2552C75.2735 17.9648 79.3347 21.5619 82.5849 25.841C84.9175 28.9121 86.7997 32.2913 88.1811 35.8758C89.083 38.2158 91.5421 39.6781 93.9676 39.0409Z"
                      fill="currentColor"
                    />
                  </svg>
                  Loading...
                </button>
              </form>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script setup>
import { ref } from "vue";

const WEB3FORMS_ACCESS_KEY = "117674fe-a6a9-4a46-8684-2114a5a92860";
const isLoading = ref(false);
const formData = ref({
  email: "",
  subject: "",
  message: "",
});
const resetFormData = () => {
  formData.value = {
    email: "",
    subject: "",
    message: "",
  };
};

const submitForm = async () => {
  isLoading.value = true;
  const response = await fetch("https://api.web3forms.com/submit", {
    method: "POST",
    headers: {
      "Content-Type": "application/json",
      Accept: "application/json",
    },
    body: JSON.stringify({
      access_key: WEB3FORMS_ACCESS_KEY,
      email: formData.value.email,
      subject: formData.value.subject,
      message: formData.value.message,
    }),
  });
  const result = await response.json();
  if (result.success) {
    console.log(result);
    resetFormData();
    isLoading.value = false;
  }
};
</script>

<style lang="scss" scoped></style>
