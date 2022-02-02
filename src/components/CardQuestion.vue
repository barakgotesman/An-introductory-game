<template>
  <div class="qCard">
    <p>נסיון</p>
  </div>
</template>
<script>
export default {
  name: 'CardQuestion',
  props: {
    card: String,
  },
};
</script>

<style scoped>
.qCard {
  position: relative;
  float: left;
  margin-right: 10px;
  width: 250px;
  height: 320px;
  border-radius: 10px;
  background: #fff;
  -webkit-box-shadow: 3px 3px 7px rgba(0, 0, 0, 0.3);
  box-shadow: 3px 3px 7px rgba(0, 0, 0, 0.3);
}
.qCard p {
  text-align: center;
  font: 100px/220px Georgia, Times New Roman, serif;
}
</style>
