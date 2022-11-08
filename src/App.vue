<script>
export default {

}
</script>

<template>
  <h1>La mia app</h1>

  <section class="main-section">
    <h2>Titolo main</h2>
    <div class="secondary-title">
      Titolo secondario
      <h2>Paragrafo</h2>
    </div>
  </section>

  <section>
    <h2>Altro titolo</h2>
    <a href="" class="link">Link</a>

    <button class="btn btn-primary">My button</button>
  </section>
  <section class="large-section">
    <h2>Titolo della sezione centrato</h2>
  </section>

  <section class="cards">
    <div class="card">
      <h2>Mia card</h2>
    </div>
    <div class="card">
      <h2>Mia card</h2>
    </div>
    <div class="card">
      <h2>Mia card</h2>
    </div>
  </section>
</template>

<style lang="scss">
@use "./style/general.scss" as *;
@use "./style/partials/variables" as *;
@use "./style/partials/mixins" as *;
// .main-section {
//   background-color: yellow;
// }
// 
// .main-section h2 {
//   color: red;
// }

.main-section {
  background-color: yellow;

  h2 {
    color: red;
  }

  .secondary-title {
    font-size: 2rem;

    p {
      color: green;
    }
  }
}

// .link {
//   color: orange;
// }
// 
// .link:hover {
//   color: green;
// }

.link {
  color: orange;

  &:hover {
    color: green;
  }
}

.btn {
  border-radius: 10px;
  padding: .5rem 1rem;

  &-primary {
    background-color: $primary-color;
  }

  &-secondary {}
}

.large-section {

  position: relative;
  height: 50vh;
  background-color: lightblue;

  @include respond('md') {
    background-color: lightgreen;
  }

  h2 {
    color: blueviolet;
    @include abs-center();
  }
}

.cards {
  @include flex(row, space-between, center);

  .card {
    position: relative;
    width: 30%;
    height: 200px;
    background-color: pink;

    h2 {
      @include abs-center();
    }
  }
}
</style>