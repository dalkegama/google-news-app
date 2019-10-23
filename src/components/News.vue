<template>
  <div>
    <input type="button" value="GetNews" @click="getNews" />
  </div>
</template>

<script>
import { data } from "@/shared/data";
export default {
  name: "news",
  props: {
    msg: String
  },
  methods: {
    getNews() {
      data.getNewsFeed();
    }
  }
};
</script>

<style scoped>
</style>
