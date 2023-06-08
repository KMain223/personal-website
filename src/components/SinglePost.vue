<template>
<router-link class="post" :to="{ name: 'Details', params: { slug: post.slug }}">
  <div class="post">
      {{ post.date }} - {{ post.title }}  <span>#{{ post.tag }}</span>
  </div>
  </router-link>
</template>

<script>
import { } from 'vue'
export default {
    props: ['post'],
}
</script>

<style>
.post {
    color: #9c9c9c;
    padding: 10px 0px;
    text-align: left;
    display: fixed;
    text-decoration: none;
    margin: 0px;
    font-size: 20px;
    font-weight: bold;
}
.post a {
    color: #bababa;
    font-weight: bold;
}
.post span {
  font-weight: normal;
  color: #787878;
}
.post:hover {
  border-top-style: solid;
  border-bottom-style: solid;
  border-top-width: 1px;
  border-bottom-width: 1px;
}
</style>