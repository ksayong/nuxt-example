<template>
  <section class="textButton">
    <div class="inner">
      <p class="textButton_text">
        Lorem ipsum dolor sit amet consectetur, adipisicing elit. Nam
        exercitationem odit voluptates laboriosam incidunt, eligendi pariatur
        voluptas eaque itaque! Eaque quibusdam qui quis at. Excepturi porro eius
        pariatur dolorum voluptate? Lorem ipsum dolor sit amet consectetur
        adipisicing elit. Vel, saepe voluptas! Minus corporis, quasi tenetur
        quia recusandae magnam molestiae tempore veniam nisi optio? Consequatur
        laboriosam incidunt a expedita nam velit.
      </p>
      <div class="btn_wrapper">
        <Button01 url="https://example.com" text="外部サイトへ" color="green" />
      </div>
      <!-- <div class="btn_wrapper">
        <Button01 url="https://example.com" text="外部サイトへ" color="blue" />
      </div>
      <div class="btn_wrapper">
        <Button01 url="https://example.com" text="外部サイトへ" color="red" />
      </div> -->
    </div>
  </section>
</template>

<script>
export default {}
</script>

<style lang="scss" scoped>
@import '@/assets/styles/app';

.btn_wrapper {
  margin: 0 auto;
  margin-top: 50px;
  max-width: 300px;
  width: 100%;
}

.textButton_text {
  border: 3px solid #cfe8e0;
  border-radius: 5px;
  display: block;
  font-size: 1.8rem;
  padding: 50px 30px;
}
</style>
