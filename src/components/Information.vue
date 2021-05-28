<template>
  <div class="info">
    <div class="title">
      <h2>Hi, I'm Yağmur!</h2>
    </div>

    <div class="desc">
      <p>
        I'm a developer. Why I choose CS? Because creating things excites me. My
        motivation is writing a memorable line. I love to share & write about
        tech.
      </p>
    </div>
  </div>
</template>

<script>
export default {
  name: "Information",
};
</script>

<style scoped>
.info {
  justify-content: center;
  align-items: center;
  display: flex;
  flex-direction: column;
}

.title {
  margin-bottom: 10px;
}

p {
  text-align: center;
  font-size: 20px;
  line-height: 30px;
}
</style>
