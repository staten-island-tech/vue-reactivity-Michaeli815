<script setup>
import CardItem from "../components/CardItem.vue";
import AddButton from "../components/AddButton.vue";

export default {
  data() {
    return {
      selected: "",
      stock: [
        {
          name: "Soccer ball",
          image: "../assets/Soccerball.jpg",
          price: "$167",
        },
        {
          name: "Basketball",
          image: "../assets/Basketball.jpg",
          price: "$98",
        },
        {
          name: "Baseball",
          image: "../assets/Baseball.jpg",
          price: "$29",
        },
        {
          name: "Hockey Puck",
          image: "../assets/Hockeypuck.jpg",
          price: "$53",
        },
        {
          name: "Football",
          image: "../assets/Football.jpg",
          price: "$45",
        },
        {
          name: "Tennis ball",
          image: "../assets/Tennisball.jpg",
          price: "$5",
        },
        {
          name: "Ping Pong Ball",
          image: "../assets/PingPongball.jpg",
          price: "$12",
        },
        {
          name: "Bowling Ball",
          image: "../assets/Bowlingball.jpg",
          price: "",
        },
        {
          name: "Volleyball Ball",
          image: "../assets/VolleyballBall.jpg",
          price: "$1",
        },
        {
          name: "Golf Ball",
          image: "../assets/GolfBall.jpg",
          price: "$19",
        },
      ],
    };
  },
};
</script>

<template>
  <main>
    <CardItem v-for="card in stock" :key="stock.name" title="stock.name" />
  </main>
  <AddButton />
  <HeadTag />
</template>
