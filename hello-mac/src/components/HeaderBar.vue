<template>
  <div class="header-wrapper">
      <div class="left-content">
          <!-- Logo + Title Here -->
          {{ title }}
      </div>

      <div class="right-content">
          <!-- Nav Properties -->
          <span>
              Reviews
          </span>

          <span>
              Places
          </span>

          <span>
              Account
          </span>

      </div>
  </div>
</template>

<script>
import 'vue-awesome/icons'
import Icon from 'vue-awesome/components/Icon'

export default {
  name: 'HeaderBar',
  components: {
    Icon
  },
  data () {
    return {
      title: 'Packatu',
      navProps: []
    }
  },
  methods: {}
}
</script>

<style scoped lang="scss">
.header-wrapper {
    display: flex;
    height: 45px;
    align-items: center;
    padding: 0 44px;
    max-width: 1280px;
    margin: 30px auto;
    box-sizing: border-box;
    .left-content {
        justify-content: flex-start;
        flex: 1;
        display: flex;
    }
    .right-content {
        justify-content: space-evenly;
        flex: 1;
        display: flex;
    }
}
</style>
