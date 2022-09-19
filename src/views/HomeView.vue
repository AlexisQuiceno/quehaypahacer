<template>
  <div>
    <div>
      <CarruselCom />
    </div>
    <div class="dd">
      <div class="card1">
        <card-component />
        <card-component />
        <card-component />
        <card-component />
      </div>
    </div>
  </div>
</template>

<script>
// @ is an alias to /src
import CarruselCom from "@/components/CarruselCom.vue";
import CardComponent from "@/components/CardComponent.vue";

export default {
  components: {
    CarruselCom,
    CardComponent,
  },
};
</script>cd

<style scoped>
.card1 {
  width: 100%;

  margin-top: 20px;
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  grid-template-rows: repeat(3, 1fr);
}
.dd {
  margin: auto;
}
</style>
