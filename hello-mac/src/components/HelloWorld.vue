<template>
  <div>
    <div class="card">
      <div class="title">
        {{ msg }}
      </div>

      <div class="review-wrapper">
        <input v-model="review.title" placeholder="Title" class="review-item">
        <input v-model="review.place" placeholder="Place" class="review-item">
        <textarea v-model="review.content" placeholder="Review" class="review-item"></textarea>
      </div>    
    </div>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  data () {
    return {
      msg: 'Write a review...',
      review: {}
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1, h2 {
  font-weight: normal;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}

.title {
  top: -40px;
  background-color: #41b883;
  position: relative;
  width: 200px;
  border-radius: 2px;
  display: flex;
  justify-content: center;
  align-self: center;
  padding: 10px 0px;
  font-size: 16px;
  max-height: 22px;
  color: white;
}

.card {
  background-color: #00000012;
  padding: 20px;
  width: 75%;
  display: flex;
  justify-content: center;
  margin: auto;
  flex-direction: column;
}

.review-wrapper {
    top: -20px;  position: relative;


  display: flex;
  flex-direction: column;
  align-items: center;
}

.review-item {
  max-height: 50px;
  font-size: 14px;
  border: none;
  border-radius: 2px;
  padding: 6px 12px;
  margin: 5px 0;
  width: 85%;
}

textarea:focus, input:focus{
    outline: solid;
    outline-color: #41b883b5;
    outline-offset: 2px;
    outline-width: 1px;
}

@media only screen and (min-width: 500px) {
    .review-item {
        width: 295px;
    }
}

</style>
