<template>
  <div class="content-wrapper">
      <div class="welcome">WELCOME</div>
      <div class="top-three-locations">TOP THREE LOCS</div>
      <div class="categories">CATEGORIES</div>
      <div class="top-two-toilets">TOP TOILETS</div>
      <div class="more-info">MORE INFO</div>

      <!-- <Welcome></Welcome>
      <TopThreeItems></TopThreeItems>
      <CategoriesExplained></CategoriesExplained>
      <TopTowItems></TopTowItems>
      <MoreInfo></MoreInfo> -->
  </div>
</template>

<script>
import 'vue-awesome/icons'
import Icon from 'vue-awesome/components/Icon'

export default {
  name: 'HomeContent',
  components: {
    Icon
  },
  data () {
    return {
    }
  },
  methods: {}
}
</script>

<style scoped lang="scss">
.content-wrapper {
    position: relative;
    padding: 0 24px;
    box-sizing: border-box;
    max-width: 1280px;
    margin: 0 auto;
    display: grid;
    grid-template-columns: repeat(2, 1fr);
    grid-auto-rows: minmax(200px, 200px);
}

.welcome {
    grid-column-start: 1;
    grid-column-end: 2;
    grid-row-start: 1;
    grid-row-end: 3;
    background-color: lightgreen;
}

.top-three-locations {
    grid-column-start: 2;
    grid-column-end: 4;
    grid-row-start: 1;
    grid-row-end: 3;
    background-color: lightblue;
}

.categories {
    grid-column-start: 1;
    grid-column-end: 4;
    grid-row-start: 3;
    grid-row-end: 4;
    background-color: lightpink;
}

.top-two-toilets {
    grid-column-start: 1;
    grid-column-end: 2;
    grid-row-start: 4;
    grid-row-end: 6;
    background-color: lightcyan;
}

.more-info {
    grid-column-start: 2;
    grid-column-end: 4;
    grid-row-start: 4;
    grid-row-end: 6;
    background-color: lightseagreen;
}
</style>
