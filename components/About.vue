<template>
  <div
    style="background-color: #ffffff"
    class="container mx-auto flex flex-col items-center pb-8"
  >
    <h1
      class="
        aboutheading
        font-medium
        leading-tight
        sm:text-5xl
        text-3xl
        pt-6
        mb-6
        text-gray-900
      "
      style="font-family: 'DM Serif Display', serif"
    >
      <span style="color: #00db80">A</span>bout ACE
    </h1>
    <div class="grid grid-cols-3 gap-8 px-4">
      <p
        class="
          container
          col-span-3
          md:col-span-2
          text-gray-700 text-lg text-center
        "
      >
      <span id="content-desktop">
        Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod
        tempor incididunt ut labore et dolore magna aliqua. Habitant morbi
        tristique senectus et netus et malesuada fames ac. Tincidunt augue
        interdum velit euismod. Morbi leo urna molestie at. Eleifend quam
        adipiscing vitae proin sagittis nisl rhoncus mattis. Nulla facilisi
        nullam vehicula ipsum a arcu cursus vitae congue. Nunc aliquet bibendum
        enim facilisis gravida neque convallis a cras. Turpis nunc eget lorem
        dolor sed viverra ipsum. Nunc mi ipsum faucibus vitae aliquet. Fringilla
        phasellus faucibus scelerisque eleifend donec. Gravida arcu ac tortor
        dignissim convallis aenean et tortor at. Dolor sit amet consectetur
        adipiscing. Pharetra magna ac placerat vestibulum lectus mauris ultrices
        </span>
        <span id="content-mobile">
        Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod
        tempor incididunt ut labore et dolore magna aliqua. Habitant morbi
        tristique senectus et netus et malesuada fames ac. Tincidunt augue
        interdum velit euismod. Morbi leo urna molestie at. Eleifend quam
        adipiscing vitae proin sagittis nisl rhoncus mattis. Nulla facilisi
        nullam vehicula ipsum a arcu cursus vitae congue. Nunc aliquet bibendum.
        </span>
        <br>
        <button
          type="button"
          class="
            text-white
            bg-green-400
            hover:bg-green-600
            focus:ring-4 focus:ring-green-300
            font-medium
            rounded-full
            text-2xl
            p-2.5
            text-center
            inline-flex
            items-center
            mr-2
            mt-4
            dark:bg-green-400 dark:hover:bg-green-600 dark:focus:ring-green-800
            rounded-full
            items-center
          "
        >
          <svg
            class="w-7 h-7"
            fill="currentColor"
            viewBox="0 0 20 20"
            xmlns="http://www.w3.org/2000/svg"
          >
            <path
              fill-rule="evenodd"
              d="M10.293 3.293a1 1 0 011.414 0l6 6a1 1 0 010 1.414l-6 6a1 1 0 01-1.414-1.414L14.586 11H3a1 1 0 110-2h11.586l-4.293-4.293a1 1 0 010-1.414z"
              clip-rule="evenodd"
            ></path>
          </svg>
        </button>
      </p>
      <img
        src="https://flowbite.com/docs/images/blog/image-1.jpg"
        class="ax-w-full rounded-lg border-4 hover:border-green-300" style="height: 250px;" id="content-desktop"
      />
    </div>
  </div>
</template>

<script>
export default {
  mounted() {
    this.animateOnScroll();
  },

  methods: {
    animateOnScroll() {
      this.$gsap.to(".aboutheading", {
        x: -300,
        ease: "Power2.easeInOut",
        scrollTrigger: {
          trigger: "bottom",
          pin: true,
          end: "bottom",
          scrub: true,
        },
      });
    },
  },
};
</script>

<style>
@import url("https://fonts.googleapis.com/css2?family=DM+Serif+Display&display=swap");
</style>