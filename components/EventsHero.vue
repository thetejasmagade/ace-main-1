<template>
  <div>
      <div style="background-color: #001e26" class="pt-12 pb-4 md:pb-0">
      <div
        class="
          container
          mx-auto
          flex flex-col
          items-center
          py-14
          sm:py-12
          mb-0
          pb-0
        "
      >
        <div class="w-11/12 sm:w-2/3 mb-5 sm:mb-10">
          <h1
            class="
              text-4xl
              sm:text-5xl
              md:text-5xl
              lg:text-6xl
              xl:text-7xl
              text-center text-white
              leading-tight
              tracking-wide
            "
            style="font-family: 'DM Serif Display', serif"
          >
            Even<span style="color: #00db80">t</span>s
          </h1>
          <p
            class="
              mt-3
              sm:mt-8
              pt-2
              text-gray-400
              font-normal
              text-center text-xl
              sm:text-2xl
            "
          >
            Develop Your Skills, Learn Something New, and Grow Your Skills With
            Association of Coders and Encoders.
          </p>
        </div>
        <div class="flex justify-center items-center">
          <NuxtLink to="join">
            <button
              class="
                focus:outline-none
                transition
                duration-150
                ease-in-out
                text-white
                hover:bg-green-600
                rounded-full
                text-white
                px-8
                sm:px-12
                py-1
                sm:py-2
                text-lg
                bg-gradient-to-r
                from-green-400
                to-blue-500
                hover:from-pink-500 hover:to-yellow-500
                font-semibold
              "
              style="background-color: #4ce6a7"
            >
              Join Club
            </button>
          </NuxtLink>
        </div>
      </div>
    </div>
    <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 1440 100" transform="rotate(180)" class="m-0 p-0" style="margin: -1px 0 -1px 0">
            <path fill="#001e26" d="M1260,1.65c-60-5.07-119.82,2.47-179.83,10.13s-120,11.48-180,9.57-120-7.66-180-6.42c-60,1.63-120,11.21-180,16a1129.52,1129.52,0,0,1-180,0c-60-4.78-120-14.36-180-19.14S60,7,30,7H0v93H1440V30.89C1380.07,23.2,1319.93,6.15,1260,1.65Z"></path>
          </svg>
  </div>
</template>

<script>
export default {

}
</script>

<style>

</style>