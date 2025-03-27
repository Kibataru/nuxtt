<template>
    <div class="main">
      <div class="banner">
        <h2>Banner</h2>
      </div>
      <div class="text">
        <h1>Hello, World!</h1>
        <p>Look at my website</p>
      </div>
      <div class="cards-blocks">
        <div class="card">
          <p>Here</p>
        </div>
        <div class="card">
          <p>And here</p>
        </div>
      </div>
    </div>
  </template>
  
  <style lang="scss" scoped>
  .main {
    max-width: 800px;
    padding: 20px;
    text-align: left;
  }

  @mixin banner-styles($bg-color, $text-color) {
    background-color: $bg-color;
    color: $text-color;
    padding: 12px 15px;
  }

  @mixin card-styles($bg-color, $text-color) {
    background-color: $bg-color;
    color: $text-color;
    padding: 8px 12px;
    min-width: 80px;
    text-align: center;
  }

  .banner {
    @include banner-styles(#1c9b33, white);
    h2 {
      margin: 0;
    }
  }

  .cards-blocks {
    display: flex;
    align-items: left;
    gap: 5px;
  }
  
  .card {
    @include card-styles(#79f19b, white);
    p {
      margin: 0;
      padding: 0;
    }
  }
  </style>