<script>
export default {
  name: "Card",
  props: {
    title: String,
    price: String,
    image: String,
  },
};
</script>

<template>
  <div class="card">
    <h2>{{ title }}</h2>
    <img src="" alt="" />
    <p>{{ price }}</p>
  </div>
</template>

<style>
.card {
  box-shadow: 10px 7px 5px rgb(255, 87, 87);
  border-radius: 3rem;
  width: %;
  height: 43rem;
  font-size: 7rem;
  background-color: rgb(228, 37, 37);
  margin: 8rem auto;
  align-items: center;
  border: 0.3rem solid rgb(107, 2, 28);
  padding: 3rem;
  display: flex;
  flex-flow: row wrap;
  justify-content: space-evenly;
}
</style>
