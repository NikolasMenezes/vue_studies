<script>

export default {
  props: {
    title: String,
    name: String,
    idade: Number,
    color: String
  }
}

</script>

<template>
  <div class="card">
    <h1 class="card-title">
      {{ title }}
    </h1>
    <p>Parabéns, {{ name }}, você tem {{ idade }} anos!</p>
  </div>
</template>

<style scoped>

  .card{
    background-color: blue;
    color: #f1f1f1;
    border: 1px solid #000;
    border-radius: 20px;
    width: 200px;
    height: 200px;
    text-align: center;
    font-size: 20px;
    margin: 10px;
    padding: 40px;
  }

</style>