<template>
  <div class="hero-section">
    <div class="nav-bar">

      <img src="../../assets/images/Authentic-Logotype.png" alt="authentic logo">

      <div class="breadcrumbs">
        <button>home</button>
        <img src="../../assets/images/icons/arrow-right.svg" alt="arrow icon">
        <button>industries</button>
        <img src="../../assets/images/icons/arrow-right.svg" alt="arrow icon">
        <button class="gray">fintech</button>
      </div>

      <div class="right-group">
      <button class="drop-down-menu">
        Services
        <img src="../../assets/images/icons/arrow-down.svg" alt="arrow icon">
      </button>
        <button>CTO Pick</button>
        <button>Case Studies</button>
        <button>About</button>
        <ColorBackgroundButton
            :text-color="TextColor.black"
            :background-color="BackgroundColor.yellow"
        >Contact us</ColorBackgroundButton>
      </div>
    </div>

  <div class="main-section">
    <div class="wrapper">
      <div class="left-group">
        <div class="header">
          Kick-start your <span>Fintech Project</span> with a team that feels like yours
        </div>

        <ColorBackgroundButton
            :text-color="TextColor.white" :background-color="BackgroundColor.blue"
        >Schedule a free expert session</ColorBackgroundButton>
      </div>

      <div class="right-group">

        <img src="../../assets/images/desktop.png" alt="desktop image">

        <img class="square-pattern" src="../../assets/images/squarePrint.svg" alt="square pattern">
      </div>

      <img class="cube" src="../../assets/images/cube.png" alt="cube image">
    </div>
  </div>

  </div>
</template>

<script setup lang='ts'>
import ColorBackgroundButton from "@/components/ColorBackgroundButton.vue";
import {BackgroundColor, TextColor} from "@/enums/ColorBackgroundButtonModifiers"

</script>

<style lang='scss' scoped>
.hero-section {


  .nav-bar{
    height: 130px;
    padding: 0 184px;
    display: flex;
    justify-content: space-between;
    align-items: center;
    position: relative;

    .breadcrumbs {
      width: 100%;
      height: 80px;
      padding: 0 184px;
      position: absolute;
      top: 84px;
      left: 0;
      display: flex;
      align-items: center;
      gap: 24px;

      button {
        font-size: $font-12px;
        font-family: "neue-montreal-regular", serif;
        color: $light-blue;
        text-transform: uppercase;
        letter-spacing: 1px;
      }

      .gray {
        color: $light-gray;
      }

    }

    .right-group {
      width: 687px;
      height: 48px;
      display: flex;
      align-items: center;
      gap: 64px;

      .drop-down-menu {
        img {
          margin-left: 8px;
        }
      }
    }
  }

  .main-section {
    padding: 33px 40px 0 40px;

    .wrapper {
      height: 674px;
      display: flex;
      background-color: $dirty-w;
      clip-path: polygon(0 80px, 80px 80px, 80px 0%, 100% 0, 100% 100%, 0 100%);
      overflow: hidden;
      position: relative;

      .left-group {
        margin-top: 160px;
        margin-left: 307px;

        .header {
          max-width: 704px;
          margin-bottom: 46px;
          font-family: "neue-montreal-regular", serif;
          font-size: $font-64px;
          color: $dark-blue;

          span {
            font-family: "gosha-sans-bold",  serif;
          }
        }
      }

      .right-group {
        margin-top: 147px;
        right: 77px;

        .square-pattern {
          width: 355px;
          height: 353px;
          position: absolute;
          top: 58px;
          right: 78px;
        }
      }

      .cube {
        width: 1011px;
        height: 1008px;
        position: absolute;
        left: -750px;
        top: 100px;
      }

    }
  }
}
</style>