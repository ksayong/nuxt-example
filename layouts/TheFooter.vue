<template>
  <div class="footer">
    <div class="inner">
      <p>footer</p>
    </div>
  </div>
</template>

<script>
export default {
  name: 'TheFooter',
}
</script>
<style lang="scss">
.footer {
  background-color: #2f495e;
  padding: 100px 0;
  width: 100%;

  .inner {
    display: flex;
    max-width: 1000px;
  }
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
