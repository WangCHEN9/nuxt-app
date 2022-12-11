<template>
  <div>
    <h2>About</h2>
    <p>
      How a user interacts with and experiences your website will determine your
      impact. Utility, ease of use, and efficiency are key.
    </p>
    <p>
      How a user interacts with and experiences your website will determine your
      impact. Utility, ease of use, and efficiency are key.
    </p>
    <div>{{ data }}</div>
  </div>
</template>

<script setup>
const { data } = await useFetch('/api/ninja?name=mario', {
  method: 'post',
  body: { age: 30 },
});
</script>

<style scoped>
h2 {
  margin-bottom: 20px;
  font-size: 36px;
}
p {
  margin: 20px 0;
}
</style>
