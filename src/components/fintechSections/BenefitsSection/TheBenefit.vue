<template>
  <div class="benefit">
    <div class="icon"><slot name="icon"></slot></div>
    <div class="title"><slot name="title"></slot></div>
    <div class="content"><slot name="content"></slot></div>
  </div>
</template>

<script setup lang='ts'>

</script>

<style lang='scss' scoped>
.benefit {
  width: 392px;
  height: 416px;
  padding: 64px 48px;
  display: flex;
  flex-direction: column;
  gap: 32px;
  z-index: 1;
  background-color: $primary-w;

  .icon {
    width: 48px;
    height: 48px;
  }

  .title {
    font-size: $font-24px;
    color: $dark-blue;
  }

  .content {
    font-family: "neue-montreal-regular", serif;
    font-size: $font-18px;
    color: $light-blue;
    line-height: 28px;
  }
}
</style>