<template>
  <header class="header">
    <h1>Текст для хедера</h1>
    <nav>
      <NuxtLink to="/">1-я часть дз</NuxtLink>
      <NuxtLink to="/blocks">2-я часть дз</NuxtLink>
    </nav>
  </header>
</template>

<style lang="scss" scoped>
.header {
  background-color: #92d6e3;
  padding: 16px;
  text-align: center;
  color: aliceblue;
  border-radius: 10px;

  a{
    color: white;
    text-decoration: none;
    margin: 0 10px;
  }
}

</style>
