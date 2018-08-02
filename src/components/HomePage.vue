<template>
  <div :class="$style.wrapper">
    <div :class="[$style.title, $style.titleColor]">
      {{ title }}
    </div>
    <div :class="[$style.title, $style.titleColor]">
      {{ secondTitle }}
    </div>
    <div :class="[$style.title, $style.titleColor]">
      {{ thirdTitle }}
    </div>
  </div>
</template>

<script>
import { camelCase, kebabCase, capitalize } from 'lodash';
export default {
  name: 'HomePage',
  computed: {
    title() {
      return camelCase('main caption');
    },
    secondTitle() {
      return kebabCase('second optional title');
    },
    thirdTitle() {
      return capitalize('third optional title');
    }
  }
};
</script>

<style lang="scss" module>
@import '../styles/index.scss';
.wrapper {
  margin: 2rem 0;
}
.title {
  font-weight: 700;
  @include mq($until: smartphone) {
    font-size: 1.6rem;
  }
  @include mq($from: smartphone) {
    font-size: 2rem;
  }
}
.titleColor {
  color: green;
}
</style>
