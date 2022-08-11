<script> 
    export default {};
</script>
<template>
      <div class="">
        <section class=" overflow-hidden">
          <div class="relative overflow-hidden bg-no-repeat bg-cover" style=" height: 600px;" :style="headerStyle">
            <div class="absolute top-0 right-0 bottom-0 left-0 w-full h-full overflow-hidden bg-fixed" >
              <div class="flex justify-center items-center h-full">
                <div class="text-center text-white px-6 md:px-12">
                  <h1 class="text-5xl md:text-6xl xl:text-7xl font-bold tracking-tight mb-12">Comming soon...<br /></h1>
                                  </div>
              </div>
            </div>
          </div>

          <div class="-mt-2.5 md:-mt-4 lg:-mt-6 xl:-mt-10" style="height: 50px; transform: scale(2); transform-origin: top center; color: #fff;">
            <svg viewBox="0 0 2880 48" xmlns="http://www.w3.org/2000/svg">
              <path d="M 0 48 L 1437.5 48 L 2880 48 L 2880 0 L 2160 0 C 1453.324 60.118 726.013 4.51 720 0 L 0 0 L 0 48 Z" fill="currentColor"></path>
            </svg>
          </div>
        </section>
      </div>
</template>
<script setup> 
  import headerImgUrl from '../assets/hero.png'
  const headerStyle = `background-image: url(${headerImgUrl});`
</script>