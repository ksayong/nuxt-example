<template>
  <div class="header">
    <div class="inner">
      <h1 class="logo">LOGO</h1>
      <ul class="header_list">
        <li><NuxtLink to="/about">menu01</NuxtLink></li>
        <li><NuxtLink to="/about">menu02</NuxtLink></li>
        <li><NuxtLink to="/about">menu03</NuxtLink></li>
      </ul>
    </div>
  </div>
</template>

<script>
export default {
  name: 'TheHeader',
}
</script>
<style lang="scss">
.header {
  background-color: #3dc58e;
  padding: 10px 0;
  position: fixed;
  width: 100%;

  .inner {
    display: flex;
    max-width: 1000px;
  }
}

.logo {
  vertical-align: middle;
}

.header_list {
  display: flex;
  font-size: 2rem;
  justify-content: space-between;
  list-style: none;
  margin-left: auto;
  width: 40%;

  a {
    color: azure;
  }
}
</style>
