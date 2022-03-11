<template>
<div>
      <Navbar />
      <EventsHero />
      <UpcomingEvents />
      <HeldEvents />
      <Footer />
  </div>
</template>

<script>
import UpcomingEvents from '../components/UpcomingEvents.vue';
export default {
  components: { UpcomingEvents },};
</script>

<style>
</style>