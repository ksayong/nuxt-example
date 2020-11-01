<template>
  <div class="footer">
    <div class="inner">
      <!-- <p>&copy; 2020 All Rights Reserved.</p> -->
      <p>fotter</p>
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

  p {
    color: aliceblue;
    font-size: 1.4rem;
    text-align: center;
    width: 100%;
  }

  .inner {
    display: flex;
    max-width: 1000px;
  }
}
</style>
