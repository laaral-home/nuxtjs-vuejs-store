<template>
  <div class="news-list">
    <div v-for="item in items" :key="item.id">
      <h2>{{ item.name }}</h2>
      <p>{{ item.description }}</p>
      <b-link :to="'/news/' + item.id">Read more ...</b-link>
    </div>
  </div>
</template>

<script>
export default {
  name: 'NewsList',
  data() {
    return {
      items: [
        {
          id: 1,
          name: 'News Header 1',
          description: 'News description 1',
        },
        {
          id: 2,
          name: 'News Header 2',
          description: 'News description 2',
        },
        {
          id: 3,
          name: 'News Header 3',
          description: 'News description 3',
        },
        {
          id: 4,
          name: 'News Header 4',
          description: 'News description 4',
        },
        {
          id: 5,
          name: 'News Header 5',
          description: 'News description 5',
        },
      ],
    }
  },
}
</script>

<style lang="scss" scoped>
.news-list {
  > div {
    h2 {
      color: red;
    }

    p {
      color: green;
    }
  }
}
</style>
