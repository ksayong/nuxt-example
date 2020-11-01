<template>
  <section class="hero">
    <div class="inner">
      <div class="hero_title-wrapper">
        <h1 class="hero_title">Top Title</h1>
        <p>
          Lorem ipsum dolor sit amet consectetur adipisicing elit. Et reiciendis
          delectus inventore, laboriosam voluptatum saepe! Quod beatae iste,
          perspiciatis nobis minus expedita facilis et laudantium eos, suscipit
          natus maiores numquam!
        </p>
      </div>
    </div>
  </section>
</template>

<script>
export default {}
</script>

<style lang="scss" scoped>
@import '@/assets/styles/app';

.hero {
  background-color: #c1eede;
  background-image: url(../assets/images/test_backimage.jpg);
  background-size: cover;
  height: 100vh;
}

.hero_title-wrapper {
  align-items: center;
  background-color: #fff;
  left: 70%;
  margin: 0;
  min-width: 400px;
  opacity: 0.3;
  padding: 100px 50px;
  position: absolute;
  top: 50%;
  -ms-transform: translate(-50%, -50%);
  -webkit-transform: translate(-50%, -50%);
  transform: translate(-50%, -50%);
  width: 30%;

  p {
    margin: 0;
  }
}

.hero_title {
  font-family: $quicksand;
  font-size: 6rem;
  margin: 0 auto 20px;
}
</style>
