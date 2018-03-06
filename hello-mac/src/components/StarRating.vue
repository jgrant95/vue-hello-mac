<template>
  <div class="hello">
    <ul class="star-rating-container">
      <li class="star" v-for="(star, index) in stars" :key="index" v-on:click="updateStar(index)">
        <icon name="star" scale="2" :class="{ 'selected': star, 'disabled': disabled }" ></icon>
      </li>
    </ul>
  </div>
</template>

<script>
import 'vue-awesome/icons'
import Icon from 'vue-awesome/components/Icon'

export default {
  name: 'StarRating',
  components: {
    Icon
  },
  data () {
    return {
      stars: [true, true, true, true, false],
      disabled: false
    }
  },
  methods: {
    test: function () {
      console.log('testttttttt')
    },
    updateStar: function (index) {
      if (this.disabled) { return }

      this.stars.fill(false)
      for (let i = 0; i <= index; i++) {
        this.$set(this.stars, i, true)
      }
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
.star-rating-container {
    margin: 0;
    padding: 0;
    display: inline-block;

    .star {
      padding: 1px;
      color: #ddd;
      list-style-type: none;
      display: inline-block;
      cursor: pointer;

      .selected {
        fill: #f9d20a;
      }
      .disabled{
        fill: rgba(128, 128, 128, 0.3);
      }
    }
}
</style>
