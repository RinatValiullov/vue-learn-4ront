<template>
  <router-link to="/event/123">
    <div class="event-card">
      <span>@ {{ event.time }} on {{ event.date }}</span>
      <h4>{{ event.title }}</h4>
    </div>
  </router-link>
</template>

<script>
export default {
  name: "EventCard",
  props: {
    event: Object
  }
};
</script>

<style scoped>
.event-card {
  border: 1px solid #39495c;
  cursor: pointer;
  margin-bottom: 18px;
  padding: 20px;
  transition: transform 0.2s ease;
  width: 250px;
}
.event-card:hover {
  box-shadow: 0 3px 12px 0 rgba(0, 0, 0, 0.2);
  transform: scale(1.01);
}
</style>
