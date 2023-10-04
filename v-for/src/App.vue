<script>
import Card from './components/Card.vue'
export default {
  components:{
    Card
  },  
  data (){
    return {
      array: [
        {
          id: 1,
          title: "bncuoasncsa",
          name: "Sofia",
          idade: 20,
          color: "rainbow"
        },
        {
          id: 2,
          title: "bncuoasncsa",
          name: "Thauan",
          idade: 240,
          color: "rainbow"
        },
        {
          id: 3,
          title: "Tahuan bobão",
          name: "Sia",
          idade: 20,
          color: "rainbow"
        },
        {
          id: 4,
          title: "titulo",
          name: "Sascnaia",
          idade: 721,
          color: "rainbow"
        }
      ]
    }
  } 
}
</script>

<template>

<div class="cards-container">
    <Card
      v-for="item in array"
      :key="item.id"
      :title="item.title"
      :name="item.name"
      :idade="item.idade"
    />
  </div>

</template>

<style scoped>
  .cards-container{
    display: grid;
    grid-template-columns: 1fr 1fr 1fr 1fr;
  }
</style>
