<template>
  <span class="badge" :class="type">
    {{ text }}
  </span>
</template>

<script>
export default {
  props: ['type', 'title'],
  computed: {
    text () {
      return this.title.toUpperCase()
    }
  }
}
</script>

<style scoped>
.badge {
  background-color: #ccc;
  color: #252525;
  border-radius: 30px;
  padding: 0.5rem 1.5rem;
  display: inline-block;
  margin-right: 0.5rem;
}

.frontend {
  background-color: #42677d;
  color: #000;
}

.backend {
  background-color: #025941;
  color: #000;
}

.career {
  background-color: #76d18b;
  color: #000;
}
</style>
