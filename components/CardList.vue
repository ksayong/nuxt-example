<template>
  <section class="card">
    <div class="inner">
      <ul class="card_list">
        <li
          v-for="(cardListItem, index) in cardList"
          :key="index"
          class="card_list-item"
        >
          <div class="item_wrapper">
            <img :src="cardListItem.imgSrc" />
            <p class="card_list-text">
              {{ cardListItem.text }}
            </p>
          </div>
        </li>
      </ul>
    </div>
  </section>
</template>

<script>
export default {
  data() {
    return {
      cardList: [
        {
          imgSrc: require('@/assets/images/nuxt.png'),
          text:
            'text1: Lorem ipsum dolor sit, amet consectetur adipisicing elit. Cupiditate rerum ipsam deserunt voluptatibus repudiandae aliquid aperiam quisquam illo consectetur cum, quod perferendis ipsum praesentium totam atque voluptatem itaque nihil ut.',
        },
        {
          imgSrc: require('@/assets/images/nuxt.png'),
          text:
            'text2: Lorem ipsum dolor sit, amet consectetur adipisicing elit. Cupiditate rerum ipsam deserunt voluptatibus repudiandae aliquid aperiam quisquam illo consectetur cum, quod perferendis ipsum praesentium totam atque voluptatem itaque nihil ut.',
        },
        {
          imgSrc: require('@/assets/images/nuxt.png'),
          text:
            'text3: Lorem ipsum dolor sit, amet consectetur adipisicing elit. Cupiditate rerum ipsam deserunt voluptatibus repudiandae aliquid aperiam quisquam illo consectetur cum, quod perferendis ipsum praesentium totam atque voluptatem itaque nihil ut.',
        },
      ],
    }
  },
}
</script>

<style lang="scss" scoped>
@import '@/assets/styles/app';

.card {
  padding: 50px 0;
}

.card_list {
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
}

.card_list-item {
  background-color: #fff;
  border: 2px solid #cfe8e0;
  border-radius: 5px;
  display: flex;
  justify-content: center;
  margin-left: 20px;
  min-width: 360px;
  padding: 20px;
  width: 30%;

  &:first-of-type {
    margin-left: 0;
  }

  img {
    margin: 0 auto;
    max-width: 300px;
    width: 100%;
  }
}

.card_list-text {
  margin: 10px auto;
}
</style>
