<template>
  <section class="card">
    <div class="inner">
      <ul class="card_list">
        <li class="card_list-item">
          <div class="item_wrapper">
            <img src="~/assets/images/nuxt.png" />
            <p class="card_list-text">
              Lorem ipsum dolor sit, amet consectetur adipisicing elit.
              Cupiditate rerum ipsam deserunt voluptatibus repudiandae aliquid
              aperiam quisquam illo consectetur cum, quod perferendis ipsum
              praesentium totam atque voluptatem itaque nihil ut.
            </p>
          </div>
        </li>
        <li class="card_list-item">
          <div class="item_wrapper">
            <img src="~/assets/images/nuxt.png" />
            <p class="card_list-text">
              Lorem ipsum dolor sit, amet consectetur adipisicing elit.
              Cupiditate rerum ipsam deserunt voluptatibus repudiandae aliquid
              aperiam quisquam illo consectetur cum, quod perferendis ipsum
              praesentium totam atque voluptatem itaque nihil ut.
            </p>
          </div>
        </li>
        <li class="card_list-item">
          <div class="item_wrapper">
            <img src="~/assets/images/nuxt.png" />
            <p class="card_list-text">
              Lorem ipsum dolor sit, amet consectetur adipisicing elit.
              Cupiditate rerum ipsam deserunt voluptatibus repudiandae aliquid
              aperiam quisquam illo consectetur cum, quod perferendis ipsum
              praesentium totam atque voluptatem itaque nihil ut.
            </p>
          </div>
        </li>
      </ul>
    </div>
  </section>
</template>

<script>
export default {}
</script>

<style lang="scss" scoped>
@import '@/assets/styles/app';

.card {
  padding: 50px 0;
}

.card_list {
  display: flex;
}

.card_list-item {
  background-color: azure;
  display: flex;
  justify-content: center;
  margin-left: 20px;
  padding: 20px;
  width: 30%;

  &:first-of-type {
    margin-left: 0;
  }

  img {
    width: 100%;
  }
}

.card_list-text {
  margin: 10px auto;
}
</style>
