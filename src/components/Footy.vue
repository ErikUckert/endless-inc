<script>
import Imprint from './Imprint.vue'
import Privacy from './Privacy.vue'
export default {
  components: {
    Imprint,
    Privacy
  }
}
</script>
<template>
  <div class="container mt-24 px-6 mx-auto max-w-2xl" id="footy">
<img src="../assets/BMWK.svg" alt="">
  </div>

  <div class="container my-10 px-6 mx-auto" id="footy">

    <details class="open:bg-gray-300 duration-300">
        <summary class="bg-inherit px-5 py-3 text-sm text-gray-500 dark:text-gray-400 cursor-pointer">Imprint</summary>
        <div class="bg-white px-5 py-3 border border-gray-300 text-sm font-light">
            <Imprint></Imprint>
        </div>
    </details>
    <details class="open:bg-gray-300 duration-300">
        <summary class="bg-inherit px-5 py-3 text-sm text-gray-500 dark:text-gray-400 cursor-pointer">Privacy</summary>
        <div class="bg-white px-5 py-3 border border-gray-300 text-sm font-light">
          <Privacy></Privacy>
        </div>
    </details>
    <br>
    <span class="text-sm text-gray-500 sm:text-center dark:text-gray-400"
      >© 2022 <a href="" class="hover:underline">Endless Industries</a>
    </span>
    <br />
    <span class="text-sm text-gray-500 sm:text-center dark:text-gray-400"
      >This website is made with &#9829; by
      <a href="https://uckert.dev/" class="hover:underline">Erik Uckert</a>.
    </span>
  </div>
</template>
