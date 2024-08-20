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
                welcome.
              </p>
            </div>
            <div
              class="grid grid-cols-1 gap-y-10 gap-x-16 sm:grid-cols-2 mt-10 mb-10"
            >
              <div class="flex gap-3 items-center">
                <div class="border-2 p-1 rounded-full shadow-sm">
                  <div class="p-3 rounded-full bg-[#f2f6fa]">
                    <svg
                      width="30"
                      height="30"
                      viewBox="0 0 24 24"
                      fill="none"
                      xmlns="http://www.w3.org/2000/svg"
                    >
                      <path
                        fill-rule="evenodd"
                        clip-rule="evenodd"
                        d="M3.75 5.25L3 6V18L3.75 18.75H20.25L21 18V6L20.25 5.25H3.75ZM4.5 7.6955V17.25H19.5V7.69525L11.9999 14.5136L4.5 7.6955ZM18.3099 6.75H5.68986L11.9999 12.4864L18.3099 6.75Z"
                        fill="#080341"
                      />
                    </svg>
                  </div>
                </div>
                <div>
                  <p class="text-base font-medium dark:text-gray-100">Email</p>
                  <p
                    class="text-sm font-normal text-gray-500 dark:text-gray-400"
                  >
                    fjlopez259@gmail.com
                  </p>
                </div>
              </div>
              <div class="flex gap-3 items-center">
                <div class="border-2 p-1 rounded-full shadow-sm">
                  <div class="p-3 rounded-full bg-[#f2f6fa]">
                    <svg
                      width="30"
                      height="30"
                      viewBox="0 0 24 24"
                      fill="none"
                      xmlns="http://www.w3.org/2000/svg"
                    >
                      <path
                        fill-rule="evenodd"
                        clip-rule="evenodd"
                        d="M6.00745 3.40686C7.68752 1.72679 10.5227 1.85451 11.6925 3.95063L12.3415 5.11356C13.1054 6.48238 12.7799 8.20946 11.6616 9.34143C11.6467 9.36184 11.5677 9.47677 11.5579 9.67758C11.5454 9.93391 11.6364 10.5267 12.5548 11.4451C13.4729 12.3632 14.0656 12.4545 14.3221 12.442C14.5231 12.4322 14.6381 12.3533 14.6585 12.3383C15.7905 11.2201 17.5176 10.8945 18.8864 11.6584L20.0493 12.3075C22.1454 13.4773 22.2731 16.3124 20.5931 17.9925C19.6944 18.8911 18.4995 19.6896 17.0953 19.7429C15.0144 19.8218 11.5591 19.2844 8.13735 15.8626C4.71556 12.4408 4.17818 8.98556 4.25706 6.90463C4.3103 5.50044 5.10879 4.30552 6.00745 3.40686ZM10.3827 4.68163C9.78363 3.60828 8.17394 3.36169 7.06811 4.46752C6.29276 5.24287 5.7887 6.09868 5.75599 6.96146C5.6902 8.6968 6.11864 11.7226 9.19801 14.8019C12.2774 17.8813 15.3031 18.3097 17.0385 18.2439C17.9013 18.2112 18.7571 17.7072 19.5324 16.9318C20.6382 15.826 20.3916 14.2163 19.3183 13.6173L18.1554 12.9683C17.432 12.5645 16.4158 12.7023 15.7025 13.4156L15.7023 13.4158C15.6322 13.4858 15.1864 13.9018 14.395 13.9403C13.5847 13.9797 12.604 13.6156 11.4942 12.5058C10.384 11.3956 10.02 10.4146 10.0597 9.60423C10.0985 8.81271 10.5147 8.36711 10.5843 8.29746L10.5844 8.29743C11.2977 7.58411 11.4354 6.56797 11.0317 5.84456L10.3827 4.68163Z"
                        fill="#1C274C"
                      />
                    </svg>
                  </div>
                </div>
                <div>
                  <p class="text-base font-medium dark:text-gray-100">
                    Contact no.
                  </p>
                  <p
                    class="text-sm font-normal text-gray-500 dark:text-gray-400"
                  >
                    09102075875
                  </p>
                </div>
              </div>
            </div>
            <div class="border"></div>
            <div class="mt-10">
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
                  <!-- <textarea
                    id="message"
                    rows="6"
                    class="block p-2.5 w-full text-sm text-gray-900 bg-gray-50 rounded-lg shadow-sm border border-gray-300 focus:ring-primary-500 focus:border-primary-500 dark:bg-gray-700 dark:border-gray-600 dark:placeholder-gray-400 dark:text-white dark:focus:ring-primary-500 dark:focus:border-primary-500"
                    placeholder="Leave a message..."
                    name="message"
                    v-model="formData.message"
                  ></textarea> -->
                  <editor
                    v-model="formData.message"
                    :init="editorConfig"
                    tinymce-script-src="../../public/tinymce/js/tinymce/tinymce.min.js"
                  ></editor>
                </div>
                <button
                  type="submit"
                  v-show="!isLoading"
                  class="duration-500 hover:scale-105 hover:shadow-xl cursor-pointer inline-flex items-center text-white bg-blue-600 hover:bg-blue-700 font-medium rounded-full text-sm px-5 py-2.5 text-center me-2 mb-2 dark:bg-blue-600 dark:hover:bg-blue-700"
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
import { ref, watch } from "vue";
import Editor from "@tinymce/tinymce-vue";

// Ref to store the editor's content
const form = ref("");

// TinyMCE editor configuration
const editorConfig = {
  placeholder: "Add important notes here",
  plugins: "advlist lists link image table",
  toolbar:
    "undo redo | formatselect | bold italic | alignleft aligncenter alignright | bullist numlist | link image media | table | outdent indent",
  menubar: false,
  branding: false,
  statusbar: false,
  paste_data_images: true,
  automatic_uploads: true,
  license_key: "gpl",
  content_security_policy: "default-src 'self'"
//   skin_url: "../../public/tinymce/js/tinymce/themes/silver",
//   content_css:
//     "../../public/tinymce/js/tinymce/skins/content/default/content.js",
};

// Watcher to monitor changes in the form ref
watch(form, () => {
  console.log(form.value);
});

// Setting the base URL for TinyMCE
// window.tinymce.baseURL = '../../public/tinymce/js/tinymce';

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
