<script setup>
import EventCard from '@/components/EventCard.vue'
import { onMounted, ref } from 'vue'

const events = ref(null)
onMounted(() => {
  //get events from mock db when component is created
})
//import TheWelcome from '../components/TheWelcome.vue'
</script>

<template>
  <main>
    <h1>Envents For Good</h1>
    <div class="events">
      <EventCard v-for="event in events" :key="event.id" :event="event" />
    </div>
  </main>
</template>

<style scoped>
.events {
  display: flex;
  flex-direction: column;
  align-items: center;
}
</style>
