<template>
  <div class="block">
    <div class="list">
      <h2>Заголовок списка</h2>
      <ul>
        <li>Опция 1</li>
        <li>Опция 2</li>
        <li>Опция 3</li>
      </ul>
    </div>

    <div class="main">
      <h2>Заголовок основного блока</h2>
      <Button />
    </div>

    <div class="third">
      <h2>Наполнение третьего блока</h2>
      <img src="/images/cat.jpg" />
    </div>
  </div>
</template>

<script setup>
import Button from "~/components/Button.vue";
</script>

<style lang="scss" scoped>
.block {
  display: flex;
  gap: 20px;
  padding: 20px;
}

.list{
  background-color: #57ae7b;
  padding: 20px;
  border-radius: 10px;
  text-align: center;
  width: 25%;
  font-family: var(--first);
}

.main{
  background-color: #f3be55;
  padding: 20px;
  border-radius: 10px;
  text-align: center;
  width: 60%;
  font-family: var(--second);
}

.third {
  background-color: #57ae7b;
  padding: 20px;
  border-radius: 10px;
  text-align: center;
  width: 25%;
  font-family: var(--first);
}

img {
  max-width: 100%;
  border-radius: 10px;
}
</style>
