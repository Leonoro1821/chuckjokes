<template>
  <div class="container my-5">
    <h1 class="text-center mb-4">Chuck Norris Jokes</h1>

    <div class="row">
      <div
        class="col-12 col-md-4 mb-4"
        v-for="(item, index) in chuck"
        :key="index"
      >
        <chuck-card
          :icon_url="item.icon_url"
          :value="item.value"
        ></chuck-card>
      </div>
    </div>
  </div>
</template>

<script>
import ChuckCard from "./components/ChuckCard.vue";

export default {
  name: "App",
  components: {
    ChuckCard,
  },
  data() {
    return {
      chuck: [
        {
          icon_url: "https://imgs.search.brave.com/jJaA5bilPQYzCSATP3Ss4sTidY1Ie1qLMxH9SiXpCWE/rs:fit:860:0:0:0/g:ce/aHR0cHM6Ly9pLnBp/bmltZy5jb20vb3Jp/Z2luYWxzLzM3LzRh/L2QyLzM3NGFkMjk0/MDMyZjQ1NjZmMDgz/NDgzNjE5YTg3NDZj/LmpwZw",
          value: "agua.",
        },
        {
          icon_url: "https://imgs.search.brave.com/jJaA5bilPQYzCSATP3Ss4sTidY1Ie1qLMxH9SiXpCWE/rs:fit:860:0:0:0/g:ce/aHR0cHM6Ly9pLnBp/bmltZy5jb20vb3Jp/Z2luYWxzLzM3LzRh/L2QyLzM3NGFkMjk0/MDMyZjQ1NjZmMDgz/NDgzNjE5YTg3NDZj/LmpwZw",
          value: "de.",
        },
        {
          icon_url: "https://imgs.search.brave.com/jJaA5bilPQYzCSATP3Ss4sTidY1Ie1qLMxH9SiXpCWE/rs:fit:860:0:0:0/g:ce/aHR0cHM6Ly9pLnBp/bmltZy5jb20vb3Jp/Z2luYWxzLzM3LzRh/L2QyLzM3NGFkMjk0/MDMyZjQ1NjZmMDgz/NDgzNjE5YTg3NDZj/LmpwZw",
          value:
            "coco.",
        },
        {
          icon_url: "https://imgs.search.brave.com/jJaA5bilPQYzCSATP3Ss4sTidY1Ie1qLMxH9SiXpCWE/rs:fit:860:0:0:0/g:ce/aHR0cHM6Ly9pLnBp/bmltZy5jb20vb3Jp/Z2luYWxzLzM3LzRh/L2QyLzM3NGFkMjk0/MDMyZjQ1NjZmMDgz/NDgzNjE5YTg3NDZj/LmpwZw",
          value: "y.",
        },
        {
          icon_url: "https://imgs.search.brave.com/jJaA5bilPQYzCSATP3Ss4sTidY1Ie1qLMxH9SiXpCWE/rs:fit:860:0:0:0/g:ce/aHR0cHM6Ly9pLnBp/bmltZy5jb20vb3Jp/Z2luYWxzLzM3LzRh/L2QyLzM3NGFkMjk0/MDMyZjQ1NjZmMDgz/NDgzNjE5YTg3NDZj/LmpwZw",
          value: "camaron.",
        },
      ],
    };
  },
};
</script>

<style>
body {
  background-color: #f8f9fa;
}
</style>
