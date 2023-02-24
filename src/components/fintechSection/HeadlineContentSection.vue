<template>
  <div class="headline-content-section">

    <div class="head-visual">
      <div class="head-visual__wrapper">

        <div class="mobile-mockup-one">
          <div class="mobile-mockup-one__wrapper">
            <img src="../../assets/images/PhoneMockup-1.png" alt="phone mockup 1">
            <img class="gif" src="../../assets/images/gifs/SplitCircle.gif" alt="gif">
          </div>
        </div>

        <div class="mobile-mockup-two">
          <div class="mobile-mockup-two__wrapper">
            <img src="../../assets/images/PhoneMockup-2.png" alt="phone mockup 1">
            <img class="gif" src="../../assets/images/gifs/HomeAppliancesAnimation.gif" alt="gif">
          </div>
        </div>

        <img class="chart-image" src="../../assets/images/ChartImage.png" alt="chart image">

      </div>

    </div>

    <div class="headline-content">

      <div class="headline">
        <div>
          <div class="section-name">for who?</div>
        </div>

        <div class="title">
          Are you running a <span>Fintech Startup</span> or need <span>Revamp your product </span>?
        </div>
      </div>

      <div class="description">
        <p class="bold">If you’re in business, fintech is probably already relevant to your operations at some level. </p>

        <p>Fintech, short for Financial Technology, is a field of technology that focuses on the development and
          improvement of financial services through the use of new technologies. Our Fintech solutions include
          automation of financial processes, providing new options for customers, and enhancing the efficiency and
          quality of financial services.
          <br>
          <br>
          Our solutions include mobile apps, robo-advisors, blockchain, smart contracts, and other Artificial Intelligence-based solutions. </p>
      </div>

      <button class="read-more-button">Read more obout fintech benefits <img src="../../assets/images/icons/arrow-top.svg" alt="arrow icon"></button>

    </div>

  </div>
</template>

<script setup lang='ts'>

</script>

<style lang='scss' scoped>
.headline-content-section {
  padding: 100px 0 0 351px;
  display: flex;

  .head-visual {
    width: 494px;
    height: 492px;

    &__wrapper {
      position: relative;

      .mobile-mockup-one {
        position: absolute;
        top: 51px;

        &__wrapper {

          .gif {
            width: 175px;
            height: 178px;
            position: absolute;
            top: 28px;
            left: 50%;
            transform: translateX(-50%);
          }
        }
      }

      .mobile-mockup-two {
        position: absolute;
        left: 160px;

        &__wrapper {

          .gif {
            width: 208px;
            height: 164px;
            position: absolute;
            top: 115px;
            left: 50%;
            transform: translateX(-50%);
          }
        }
      }

      .chart-image {
        position: absolute;
        top: 120px;
        right: 0;
      }
    }
  }

  .headline-content {
    max-width: 693px;
    margin-left: 67px;

    .headline {
      display: flex;
      flex-direction: column;
      gap: 24px;

      .section-name {
        width: 70px;
        padding-bottom: 8px;
        margin-bottom: 24px;
        border-bottom: 3px solid $juicy-yellow;
        font-size: $font-12px;
        letter-spacing: 1px;
        text-transform: uppercase;
      }

      .title {
        font-size: $font-40px;
        color: $dark-blue;

        span {
          font-family: "gosha-sans-bold", serif;
        }
      }
    }

    .description {
      margin-top: 43px;
      p {
        margin: 0;
        font-family: "neue-montreal-regular", serif;
        font-size: 18px;
        color: $light-blue;
        line-height: 28px;
      }

      p.bold {
        margin-bottom: 24px;
        font-size: $font-24px;
        color: $dark-blue;
      }
    }

    .read-more-button {
      margin-top: 43px;
      padding: 15px 32px;
      color: $blue;
      border-radius: 4px;
      cursor: pointer;
      transition: $time-hover-anim;

      img {
        margin-left: 8px;
      }
    }

    .read-more-button:hover {
      background-color: rgba(122, 194, 220, 0.5);
    }
  }

}
</style>