<template>
  <button :class="colorBackgroundButtonClassName">
      <slot></slot>
  </button>
</template>

<script setup lang='ts'>
import {computed} from "vue";

const props = defineProps({
  backgroundColor: {
    type: String,
    required: true
  },
  textColor: {
    type: String,
    required: true
  }
});

const colorBackgroundButtonClassName = computed(() => {
  return "color-background-button" + " " + props.backgroundColor + " " + props.textColor
})
</script>

<style lang='scss' scoped>
.color-background-button {
  padding: 15px 32px;
  border-radius: 4px;
  transition: $time-hover-anim;
}

.color-background-button:hover {
  filter: brightness(0.9);
}

.color-background-button:active {
  filter: brightness(0.7);
  transition: $time-click-anim;
}

.color-background-button.text-black {
  color: black;
}

.color-background-button.text-white {
  color: white;
}


.color-background-button.background-yellow {
  background-color: $juicy-yellow;
}

.color-background-button.background-blue {
  padding: 23px 48px;
  background-color: $blue;
}
</style>