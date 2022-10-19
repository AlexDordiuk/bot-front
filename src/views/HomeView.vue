<script setup>
import {ref} from "vue";

const counter = ref(0);
const counter1 = ref(0);
</script>

<template>
  <main>
    <div class="container">
      <div class="top-container-box d-flex justify-content-between">
        <div class="small-card-item">
          <img src="../assets/img/photo-1.png" alt="photo 1">
          <p class="title text-center">Лляна олія</p>
          <div class="d-flex justify-content-around align-items-center">
            <span>100мл - 100грн</span>
            <button type="button" @click="() => counter--">-</button>
            {{counter}}
            <button type="button" @click="() => counter++">+</button>
          </div>
          <div class="d-flex justify-content-around align-items-center">
            <span>250мл - 200грн</span>
            <button type="button" @click="() => counter1--">-</button>
            {{counter1}}
            <button type="button" @click="() => counter1++">+</button>
          </div>
          <button type="button" class="more-btn">детальніше</button>
        </div>
        <div class="small-card-item">
          <img src="../assets/img/photo-1.png" alt="photo 1">
          <p class="title text-center">Лляна олія</p>
          <div class="d-flex justify-content-around align-items-center">
            <span>100мл - 100грн</span>
            <button type="button" @click="() => counter--">-</button>
            {{counter}}
            <button type="button" @click="() => counter++">+</button>
          </div>
          <div class="d-flex justify-content-around align-items-center">
            <span>250мл - 200грн</span>
            <button type="button" @click="() => counter1--">-</button>
            {{counter1}}
            <button type="button" @click="() => counter1++">+</button>
          </div>
          <button type="button" class="more-btn">детальніше</button>
        </div>

      </div>

    </div>
  </main>
</template>

<style lang="scss">
.small-card-item {
  width: 186px;
  height: 219px;
  background-color: #f9eec7;
  border-radius: 10px;
  box-shadow: 3px 3px 3px 0px rgba(0, 0, 0, 0.25);
  font-family: $neucha;
  font-weight: 400;
  color: #563725;

  img {
    width: 100%;
    height: 111px;
    border-top-left-radius: inherit;
    border-top-right-radius: inherit;
  }

  .title {
    font-size: 20px;
    line-height: 1.1;
    margin-top: 7px;
    margin-bottom: 8px;
  }

  button {
    width: 15px;
    height: 15px;
    border-radius: 50%;
    color: #dadada;
    border: none;
    outline: none;
    background-color: #563725;
    display: flex;
    justify-content: center;
    align-items: center;
    padding: 0 !important;
  }
  &>div {
    padding-left: 16px;
    padding-right: 20px;
  }

  .more-btn {
    width: 118px;
    height: 20px;
    border-radius: 30px;
    background-color: #563725;
    color: #f9eec7;
    box-shadow: 2px 2px 2px 0px rgba(0, 0, 0, 0.25);
    margin: 0 auto;
    text-transform: uppercase;
    font-size: 12px;
    letter-spacing: 1px;
  }
}
</style>