<template>
  <div class="item-wrapper">
    <div class="gradient-item" style="background: linear-gradient(90deg, #69b7eb, #b3dbd3, #f4d6db);">
      COVENTRY
    </div>
    <div class="gradient-item" style="background: linear-gradient(90deg, #cfecd0, #a0cea7, #9ec0db);">
      BIRMINGHAM
    </div>
    <div class="gradient-item" style="background: linear-gradient(90deg, #ee5c87, #f1a4b5, #d587b3);">
      LINCOLN
    </div>
  </div>
</template>

<script>
import 'vue-awesome/icons'
import Icon from 'vue-awesome/components/Icon'

export default {
  name: 'TopThreeItems',
  components: {
    Icon
  },
  data () {
    return {
    }
  },
  methods: {
  }
}
</script>

<style scoped lang="scss">
.item-wrapper {
  display: flex;
  flex-direction: column;
  margin: auto 0;
  height: 90%;
  justify-content: space-evenly;
  align-items: center;
  width: 100%;

  .gradient-item {
    flex: 1;
    width: 100%;
    margin: 8px 0;
    display: flex;
    align-items: center;
    justify-content: center;
    border-radius: 4px;
    font-size: 1.5em;
  }
}
</style>
