<template>
  <div class="card">
      <img class="image" :src="cardDetails.image" alt="" />
      <h3 class="header">
          {{cardDetails.title}}
      </h3>
      <p class="snippets">
          {{cardDetails.snippets}}
      </p>
  </div>
</template>

<script>
export default {
    props: ["cardDetails"]
};
</script>

<style scoped>
.card {
  width: 31.5%;
  height: 25rem;
  border: none;
  overflow: hidden;
  padding: 0;
  cursor: pointer;
}
.image {
  height: 65%;
  border-radius: 0.5rem;
}
.header {
  font-size: 1.15rem;
  margin-top: 0.4rem;
}
.snippet {
  color: grey;
}
</style>
