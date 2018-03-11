<template>
  <div class="content-wrapper">
      <div class="subtitle">toilets say a lot about a place.</div>
      <div class="welcome" style="display: flex; flex-direction: column;">
            <div class="text">
                Hello and welcome to the most amazing toilet reviewing website in the world. Everything is here and readily available for you. So what are you waiting for, go ahead; review and rate that toilet!
            </div>
        </div>
      <div class="top-three-locations">
          <div style="margin: auto;">TOP THREE PLACES</div>
          <TopThreeItems/>
        </div>
        <div class="top-toilet">
          <div style="margin: auto;">TOP TOILET</div>
          <TopThreeItems/>
        </div>
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
import TopThreeItems from './TopThreeItems'

export default {
  name: 'HomeContent',
  components: {
    Icon,
    TopThreeItems
  },
  data () {
    return {
    }
  },
  methods: {}
}
</script>

<style scoped lang="scss">
$content-item-inner-padding: 10px;
$content-grid-spacing: 1.0em;

.content-wrapper {
    position: relative;
    padding: 0 24px;
    box-sizing: border-box;
    max-width: 1280px;
    margin: 0 auto;
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    grid-auto-rows: minmax(86px, 86px);
    grid-gap: $content-grid-spacing;
    margin: $content-grid-spacing auto;
}

.subtitle{
    padding: $content-item-inner-padding;
    grid-column-start: 1;
    grid-column-end: 4;
    grid-row-start: 1;
    grid-row-end: 2;
    display: flex;
    align-items: center;
    justify-content: center;
    font-size: 3em;
}

.welcome {
    padding: $content-item-inner-padding;
    grid-column-start: 1;
    grid-column-end: 2;
    grid-row-start: 2;
    grid-row-end: 5;
    .text{
        justify-content: space-evenly;
        align-items: center;
        font-size: 1.3em;
        margin: auto 0;
    }
}

.top-toilet {
    padding: $content-item-inner-padding;
    grid-column-start: 3;
    grid-column-end: 4;
    grid-row-start: 2;
    grid-row-end: 5;
    display: flex;
    flex-direction: column;
    justify-content: space-evenly;
}

.top-three-locations {
    padding: $content-item-inner-padding;
    grid-column-start: 2;
    grid-column-end: 3;
    grid-row-start: 2;
    grid-row-end: 5;
    display: flex;
    flex-direction: column;
    justify-content: space-evenly;
}

.categories {
    padding: $content-item-inner-padding;
    grid-column-start: 1;
    grid-column-end: 3;
    grid-row-start: 5;
    grid-row-end: 7;
    background-color: lightpink;
    border-radius: 4px;
}

.top-two-toilets {
    padding: $content-item-inner-padding;
    grid-column-start: 1;
    grid-column-end: 2;
    grid-row-start: 7;
    grid-row-end: 10;
    background-color: lightcyan;
    border-radius: 4px;
}

.more-info {
    padding: $content-item-inner-padding;
    grid-column-start: 2;
    grid-column-end: 3;
    grid-row-start: 7;
    grid-row-end: 10;
    background-color: lightseagreen;
    border-radius: 4px;
}
</style>
