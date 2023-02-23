<template>
  <div class="digital-product-design-section">
    <div class="wrapper">
      <div class="number">31</div>
      <div class="title">Screen Designed</div>
    </div>

    <div class="wrapper">
      <div class="number">613</div>
      <div class="title">Hours of Design</div>
    </div>

    <div class="wrapper">
      <div class="flex">
        <div class="number">+24</div>
        <span class="number smaller-font">%</span>
      </div>
      <div class="title">More Clients on the website</div>
    </div>

    <div class="wrapper">
      <div class="number">144</div>
      <div class="title">Wireframes & User Flows</div>
    </div>

  </div>
</template>

<script setup lang='ts'>

</script>

<style lang='scss' scoped>
.digital-product-design-section {
  height: 234px;
  display: flex;
  justify-content: center;
  align-items: center;
  gap: 192px;

  .wrapper {

    .flex {
      display: flex;
      justify-content: center;
      align-items: center;
    }

    .number {
      font-family: "gosha-sans-bold", serif;
      font-size: $font-64px;
      text-align: center;
      color: $dark-blue;
    }

    .number.smaller-font {
      font-size: $font-24px;
    }

    .title {
      max-height: 72px;
      margin-top: 16px;
      color: $light-blue;
    }
  }
}
</style>