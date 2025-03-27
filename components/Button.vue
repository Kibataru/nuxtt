<template>
  <div>
    <p class="change">{{ hello }}</p>
    <button class="button" @click="newText">Поменять приветствие</button>
  </div>
</template>

<script setup>
import {ref} from 'vue';

const hello = ref("Всем привет!");

const newText = () => {
  const text = [
    "Вы здесь? Это странно. Что задумали?",
    "О, новый гость! Или старый... Я всё равно ничего не запоминаю.",
    "Добрый день!",
    "Работает, и это чудо!",
    "Всем привет!"
  ];
  
  let randomIndex = Math.floor(Math.random() * text.length);
  hello.value = text[randomIndex];
};
</script>

<style lang="scss" scoped>
.change {
  font-size: 18px;
  margin-bottom: 10px;
}

.button {
  background-color: #7d8d9b;
  color: aliceblue;
  padding: 10px 10px;
  border: none;
  cursor: pointer;
  border-radius: 10px;
}
</style>
