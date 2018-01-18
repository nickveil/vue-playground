<template>
  <div class="container hello">
    <h1>Vue-Playground</h1>
    <div class="card">
      <div class="row">
        <div class="col-2">
          <div class="image">
            No Photo Available
          </div>
        </div>
        <div class="col-10">
          <div><p class="name">{{ msg }}</p></div>
          <div class="address"><span>Address goes here.</span></div>
          <div class="number"><span>Phone number goes here.</span></div>
          <div class="email"><span>Email goes here.</span></div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Card',
  data () {
    return {
      msg: 'Name (First Last)'
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.card {
  position: absolute;
  border: solid 1px #000;
  height: 100px;
  width: 280px;
  border-radius: 4px;
  margin:5px;
}
.image {
  border: solid 1px #ccc;
  height: 75px;
  width: 60px;
  margin: 12px 10px;
  font-size: 12px;
  text-align: center;
}
.name{
  width: 200px;
  height: 20px;
  margin: 5px 20px;
  font-size: 18px;
  text-align: center;
}
</style>
