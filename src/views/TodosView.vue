<script setup>
import TodoHeader from "../components/TodoHeader.vue";
</script>

<template>
  <div class="container">
    <div class="row justify-content-between">
      <div class="col-4">
        <span class="update"
          ><img src="../assets/Union.svg" alt="unionlogo" /> Introducing Image
          Feature</span
        >
        <h1 class="myTitle">Imagine with Serendipity</h1>
      </div>
      <div class="col-4">One of two columns</div>
    </div>
  </div>
</template>

<style lang="scss" scoped>
.update {
  color: #fff;
  border-radius: 8px;
  background: linear-gradient(
    180deg,
    rgba(255, 255, 255, 0.1) 0%,
    rgba(255, 255, 255, 0.05) 100%
  );
  box-shadow: 0px 30px 60px 0px rgba(0, 0, 0, 0.5);
}
.myTitle {
  /* Heading/H1 */
  width: auto;
  margin-top: 15px;
  background: linear-gradient(to right, #cc51d6, #5a68e8, #e1b1ff);
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  font-size: 60px;
  font-style: normal;
  font-weight: 600;
  line-height: 60px;
}
</style>
