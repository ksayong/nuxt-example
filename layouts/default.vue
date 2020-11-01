<template>
  <div>
    <TheHeader v-if="existsHeader" />
    <Nuxt />
    <div style="display: flex; justify-content: center; padding: 100px 0">
      <div class="btn_wrapper">
        <NuxtLink to="/" class="button--green">Home</NuxtLink>
        <NuxtLink to="/about" class="button--green">About</NuxtLink>
        <NuxtLink to="/about" class="button--green">01</NuxtLink>
        <NuxtLink to="/about" class="button--green">02</NuxtLink>
        <NuxtLink to="/about" class="button--green">03</NuxtLink>
      </div>
    </div>
    <TheFooter />
  </div>
</template>

<script>
import TheHeader from './TheHeader'
// import TheFooter from './TheFooter'

export default {
  name: 'Default',
  components: {
    TheHeader,
  },
  computed: {
    existsHeader() {
      const excludedHeaderPageList = ['About']
      return !excludedHeaderPageList.includes(this.$route.name)
    },
  },
}
</script>

<style lang="scss">
@import '@/assets/styles/app';

.btn_wrapper {
  display: flex;
  justify-content: center;
  max-width: 500px;
  width: 100%;
}

.button--green {
  border: 1px solid #3b8070;
  border-radius: 4px;
  color: #3b8070;
  display: inline-block;
  font-size: 1.8rem;
  margin-left: 20px;
  padding: 10px 30px;
  text-decoration: none;
  transition: 0.8s;

  &:first-of-type {
    margin-left: 0;
  }

  &:hover {
    background-color: #3b8070;
    color: #fff;
  }
}

.button--grey {
  border: 1px solid #35495e;
  border-radius: 4px;
  color: #35495e;
  display: inline-block;
  font-size: 1.8rem;
  margin-left: 15px;
  padding: 10px 30px;
  text-decoration: none;
  transition: 0.8s;
  &:hover {
    background-color: #35495e;
    color: #fff;
  }
}
</style>
