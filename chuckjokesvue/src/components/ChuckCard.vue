<template>
  <div class="card h-100 shadow-sm">
    <img :src="icon_url" class="card-img-top p-3" alt="Chuck Norris" />
    <div class="card-body">
      <p class="card-text">{{ value }}</p>
    </div>
  </div>
</template>

<script>
export default {
  name: "ChuckCard",
  props: {
    icon_url: String,
    value: String,
  },
};
</script>

<style scoped>
.card {
  border-radius: 12px;
  transition: transform 0.3s;
}
.card:hover {
  transform: scale(1.03);
}
.card-img-top {
  width: 80px;
  height: 80px;
  object-fit: contain;
  margin: auto;
  display: block;
}
.card-text {
  text-align: center;
  font-size: 0.95rem;
}
</style>
