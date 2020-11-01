<template>
  <a
    :href="url"
    target="_blank"
    class="button"
    :class="{
      red: color === 'red',
      blue: color === 'blue',
      green: color === 'green',
    }"
    >{{ text }}</a
  >
</template>

<script>
export default {
  props: {
    url: {
      type: String,
      required: true,
    },
    text: {
      type: String,
      required: true,
    },
    color: {
      type: String,
      default: '',
    },
  },
}
</script>

<style lang="scss" scoped>
@import '@/assets/styles/app';

.button {
  background-color: black;
  border: 2px solid black;
  color: white;
  font-family: $quicksand;
  font-size: 2rem;
  padding: 20px 10px;
  text-align: center;
  transition: 0.8s;
  width: 100%;

  &:hover {
    background-color: #fff;
    color: black;
  }
}

.red {
  background-color: #ca6c6c;
  border: 2px solid #ca6c6c;

  &:hover {
    color: #ca6c6c;
  }
}

.blue {
  background-color: #414db8;
  border: 2px solid #414db8;

  &:hover {
    color: #414db8;
  }
}

.green {
  background-color: #41b883;
  border: 2px solid #41b883;

  &:hover {
    color: #41b883;
  }
}
</style>
