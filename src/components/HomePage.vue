<template>
  <div :class="$style.wrapper">
    <div :class="$style.title">
      title
    </div>
  </div>
</template>

<script>
export default {
  name: 'HomePage',
  props: {
    msg: String
  }
};
</script>

<style lang="scss" module>
.wrapper {
  margin: 2rem 0;
}
.title {
  text-transform: capitalize;
  font-weight: 700;
  font-size: 2rem;
}
</style>
