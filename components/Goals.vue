<template>
<div>
  <div
    style="background-color: #ffffff"
    class="container mx-auto flex flex-col items-center py-8"
  >
    <h1
      class="
        goalsheadingdesktop
        font-medium
        leading-tight
        sm:text-5xl
        text-3xl
        pt-6
        mb-6
        text-gray-900
      "
      style="font-family: 'DM Serif Display', serif"
      id="content-desktop"
    >Our Go<span style="color: #00db80">a</span>ls
    </h1>
    <h1
      class="
        goalsheadingmobile
        font-medium
        leading-tight
        sm:text-5xl
        text-3xl
        pt-6
        mb-6
        text-gray-900
      "
      style="font-family: 'DM Serif Display', serif"
      id="content-mobile"
    >
      <span style="color: #00db80">O</span>ur Goa<span style="color: #00db80">l</span>s
    </h1>
    <div class="grid grid-cols-3 gap-6 px-4">
      <img
        src="https://flowbite.com/docs/images/blog/image-1.jpg"
        class="ax-w-full rounded-lg border-4 hover:border-green-300 ml-12" style="height: 250px;" id="content-desktop"
      />
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
      </p>
    </div>
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
      this.$gsap.to(".goalsheadingdesktop", {
        x: 300,
        ease: "Power2.easeInOut",
        scrollTrigger: {
          trigger: "bottom",
          pin: true,
          end: "bottom",
          scrub: true,
        },
      });
      this.$gsap.to(".goalsheadingmobile", {
        x: 100,
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