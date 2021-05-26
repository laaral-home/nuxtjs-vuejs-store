<template>
  <div class="detail-news">Detail news page</div>
</template>

<script>
export default {
  mounted() {
    console.log(this.$route)
  },
}
</script>

<style lang="scss" scoped>
.detail-news {
  background-color: blue;
  color: white;
}
</style>
