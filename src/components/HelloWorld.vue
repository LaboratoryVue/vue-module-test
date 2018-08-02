<template>
  <div>
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
.title {
  text-transform: capitalize;
  font-weight: 700;
  font-size: 2rem;
}
</style>
