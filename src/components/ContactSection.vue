<script>
export default {
    name: "ContactComp",
    props: {
      showModal: Boolean,
      showContactSection: Boolean
    }
}</script>
<template>
<div v-if="showContactSection" class="container my-24 px-6 mx-auto" id="contact">
  <section class="mb-32 text-gray-800 text-center lg:text-left">
    <div class="flex flex-wrap justify-center">
      <div class="grow-0 shrink-0 basis-auto w-full lg:w-10/12 px-3">
        <div class="grid lg:grid-cols-2 gap-x-6 items-center">
          <div class="mb-10 lg:mb-0">
            <h2 class="text-3xl font-bold">
              Do not miss any updates.
              <br />
              <span class="text-gray-500">Feel free to contact us.</span>
            </h2>
          </div>

          <div class="mb-6 md:mb-0">
            <div class="xl:flex flex-row">
              <button
                type="submit"
                class="inline-block px-7 py-3 bg-gray-500 
                text-white font-medium text-sm leading-snug uppercase 
                rounded shadow-md hover:bg-gray-800 hover:shadow-lg 
                focus:bg-gray-800 focus:shadow-lg focus:outline-none 
                focus:ring-0 active:bg-blue-800 active:shadow-lg transition duration-150 ease-in-out"
                data-mdb-ripple="true"
                data-mdb-ripple-color="light"
                id="show-modal" @click="$emit('show')"
              >
                Send us a message
              </button>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>

</div>
</template>