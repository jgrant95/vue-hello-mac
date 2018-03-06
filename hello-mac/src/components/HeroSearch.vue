<template>
  <div class="hero-background">
      <div class="search-wrapper">
            <input type="text" class="search-box">
            <icon name="search" scale="1.5" class="icon-subtle"></icon>
      </div>
  </div>
</template>

<script>
import 'vue-awesome/icons'
import Icon from 'vue-awesome/components/Icon'

export default {
  name: 'HeroSearch',
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
.hero-background {
    background-color: rgba(128, 128, 128, 0.3);
    display: flex;
    height: 320px;
    position: relative;
    width: 100%;
    justify-content: center;
}

.search-wrapper {
    height: 44px;
    border-radius: 2px;
    align-self: center;
    background-color: rgba(255, 255, 255, 0.8);
    width: 700px;
    padding: 0 8px;
    position: relative;
}

.search-box {
    height: 44px;
    border: none;
    background-color: transparent;
    width: 100%;
    outline: none;
    padding: 0;
}

.icon-subtle {
    position: absolute;
    color: grey;
    opacity: 0.8;
    right: 0;
    bottom: 0;
    margin: 10px;
}
</style>
