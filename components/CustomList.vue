<template>
  <ul class="custom-list">
    <li v-for="(item, index) in items" :key="index">
      <span class="icon">☘️</span>
      <span class="text">
        <slot :item="item" :index="index">{{ item }}</slot>
      </span>
    </li>
  </ul>
</template>

<script setup>
defineProps({
  items: {
    type: Array,
    required: true,
  },
});
</script>

<style scoped>
.custom-list {
  list-style: none;
  padding: 0;
  margin: 0;
  text-align: left;
}

.custom-list li {
  display: flex;
  align-items: center;
  margin-bottom: 15px;
  font-size: 1.0rem;
  line-height: 1.8;
}

.custom-list .icon {
  margin-right: 10px;
  background: linear-gradient(90deg, #88b04b, #f4d03f);
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
}

.custom-list li strong {
    font-weight: bold;
    background: linear-gradient(90deg, #c4e17f, #f7d26d); /* สี Gradient */
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    -moz-background-clip: text;
    -moz-text-fill-color: transparent;
  }
  strong {
    font-weight: bold;
    background: linear-gradient(90deg, #c4e17f, #f7d26d); /* Gradient สี */
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    -moz-background-clip: text;
    -moz-text-fill-color: transparent;
    font-size: 1.5rem; /* ขนาดข้อความ */
    line-height: 1.8;
  }
.custom-list .text {
  color: white;
}
</style>
