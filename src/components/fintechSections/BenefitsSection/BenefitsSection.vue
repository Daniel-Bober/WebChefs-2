<template>
  <div class="benefits-section">
    <div class="benefits-section__wrapper">

      <div class="headline">
        <div class="wrapper">
          <div class="section-name">benefits for your business</div>
        </div>

        <div class="title">
          What we can do to <span>boost your fintech business?</span>
        </div>
      </div>

      <div class="hover-benefit">
        <div class="benefits-group">

          <TheBenefit class="hover-tile">
            <template v-slot:icon>
              <img src="../../../assets/images/icons/benefit-icon-1.svg" alt="benefit icon">
            </template>
            <template v-slot:title>Use data to understand your clients better</template>
            <template v-slot:content>
              Find patterns in the behavior of your customers using machine learning and forecast when they need specific products
            </template>
          </TheBenefit>


          <TheBenefit class="no-hover-tile">
            <template v-slot:icon>
              <img src="../../../assets/images/icons/benefit-icon-2.svg" alt="benefit icon">
            </template>
            <template v-slot:title>Build financial products your customers want</template>
            <template v-slot:content>
              Use intelligent platforms to replace generic products with a personalized and timely offering.t
            </template>
          </TheBenefit>

          <TheBenefit class="no-hover-tile">
            <template v-slot:icon>
              <img src="../../../assets/images/icons/benefit-icon-3.svg" alt="benefit icon">
            </template>
            <template v-slot:title>Increasing Use of AI</template>
            <template v-slot:content>
              Artificial intelligence (AI) has become an important part of many different businesses in recent years.
              The financial sector is no different.
            </template>
          </TheBenefit>
        </div>

        <div class="benefits-group">
          <TheBenefit class="no-hover-tile">
            <template v-slot:icon>
              <img src="../../../assets/images/icons/benefit-icon-4.svg" alt="benefit icon">
            </template>
            <template v-slot:title>Create a frictionless omnichannel banking experience</template>
            <template v-slot:content>
              Find patterns in the behavior of your customers using machine learning and forecast when they need specific products
            </template>
          </TheBenefit>

          <TheBenefit class="no-hover-tile">
            <template v-slot:icon>
              <img src="../../../assets/images/icons/benefit-icon-5.svg" alt="benefit icon">
            </template>
            <template v-slot:title>Improve your customer service</template>
            <template v-slot:content>
              Use intelligent platforms to replace generic products with a personalized and timely offering.t
            </template>
          </TheBenefit>

          <TheBenefit class="no-hover-tile">
            <template v-slot:icon>
              <img src="../../../assets/images/icons/benefit-icon-6.svg" alt="benefit icon">
            </template>
            <template v-slot:title>Enhance the security of transactions and data</template>
            <template v-slot:content>
              Artificial intelligence (AI) has become an important part of many different businesses in recent years.
              The financial sector is no different.
            </template>
          </TheBenefit>
        </div>

        <div class="hover-benefits-background">
          <div class="info-section">

            <div class="title">
              Discover how we <br> <span>achieved sale success</span>
            </div>

            <div class="description">
              Find patterns in the behavior of your customers using machine learning and forecast when they need specific products
            </div>

            <div class="white-square"></div>
            <div class="white-square secondary"></div>
          </div>
        </div>

      </div>

    </div>
  </div>
</template>

<script setup lang='ts'>
import TheBenefit from "@/components/fintechSections/BenefitsSection/TheBenefit.vue";

</script>

<style lang='scss' scoped>
.benefits-section {
  padding: 147px 40px 20px 40px;

  &__wrapper {
    min-height: 1250px;
    padding: 128px 308px 0 308px;
    display: flex;
    flex-direction: column;
    background-color: $dirty-w;
    clip-path: polygon(0 80px, 80px 80px, 80px 0%, 100% 0, 100% 100%, 0 100%);
    overflow: hidden;
    position: relative;

    .headline {
      display: flex;
      flex-direction: column;
      gap: 24px;

      .wrapper {
        .section-name {
          padding-bottom: 8px;
          display: inline;
          border-bottom: 3px solid $juicy-yellow;
          font-size: $font-12px;
          letter-spacing: 1px;
          text-transform: uppercase;
        }
      }

      .title {
        font-size: $font-40px;
        color: $dark-blue;

        span {
          font-family: "gosha-sans-bold", serif;
        }
      }
    }

    .hover-benefit {
      margin-top: 80px;
      max-width: 1224px;
      display: flex;
      flex-direction: column;
      gap: 24px;
      pointer-events: none;
      position: relative;

      .benefits-group {
        display: flex;
        gap: 24px;

        .hover-tile {
          z-index: 2;
          pointer-events: auto;
          cursor: pointer;
        }

        .no-hover-tile {
          transition: $time-long-hover-anim ease-in-out;
        }
      }

      .hover-benefits-background {
        width: 100%;
        height: 100%;
        position: absolute;
        pointer-events: none;
        top: 0;
        left: 0;
        background-image: url("../../../assets/images/hover-benefits-background.jpg");
        background-repeat: no-repeat;
        opacity: 0;
        transition: $time-long-hover-anim ease-in-out;

        .info-section {
          width: 820px;
          height: 440px;
          padding: 97px 0 0 153px;
          display: flex;
          flex-direction: column;
          position: absolute;
          bottom: 0;
          right: 0;
          background-color: rgba(255, 255, 255, 17%);

          .title {
            max-width: 486px;
            font-size: $font-40px;
            color: $primary-w;

            span {
              font-family: "gosha-sans-bold", serif;
            }
          }

          .description {
            max-width: 486px;
            margin-top: 24px;
            font-family: "neue-montreal-regular", serif;
            font-size: $font-18px;
            color: $primary-w;
          }

          .white-square {
            width: 40px;
            height: 40px;
            position: absolute;
            bottom: 0;
            right: 0;
            background-color: $primary-w;
          }
          .white-square.secondary {
            bottom: 40px;
            right: 40px;
          }
        }
      }
    }

    .hover-benefit:hover .no-hover-tile {
      opacity: 0;
    }

    .hover-benefit:hover .hover-benefits-background {
      opacity: 100%;
      pointer-events: auto;
      z-index: 1;
    }

    .hover-benefits-background:hover {
      opacity: 100%;
      pointer-events: auto;
      z-index: 1;
    }

    .hover-benefits-background:hover .no-hover-tile {
      opacity: 0;
    }

  }
}
</style>