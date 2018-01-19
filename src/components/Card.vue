<template>
  <div class="container hello">
    <h1>Vue-Playground</h1>
    <div class="card">
      <div class="row">
        <div class="col-2">
          <div>
            <img class="image":src="img" alt="Profile" height="90" width="90">
          </div>
        </div>
        <div class="col-10">
          <div><p class="name">{{ msg }}</p></div>
          <div class="address"><span>{{ address1 }}<br/>{{address2}}</span></div>
          <div class="number"><span>{{number}}</span></div>
          <div class="email"><span>{{ email }}</span></div>
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
      msg: 'John Smith',
      img: require('../../profile.jpeg'),
      address1: '123 Any St',
      address2: 'AnyTown, US 12345',
      number: '(555)-555-555',
      email: 'name.last@mail.com'
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
  height: 90px;
  width: 90px;
  margin: 3px 10px;
  font-size: 12px;
  text-align: center;
  border-radius: 4px;
  background-color: #eee;
}
.name{
  width: 200px;
  height: 18px;
  margin: 3px 20px;
  font-size: 18px;
  font-weight: 600;
  text-align: center;
}
.address{
  width: 200px;
  height: 30px;
  margin: 4px 20px;
  font-size: 12px;
  text-align: center;
}
.number {
  width: 200px;
  height: 14px;
  margin: 3px 20px;
  font-size: 14px;
  font-weight: 600;
  text-align: center;
}
.email{
  width: 200px;
  height: 30px;
  margin: 3px 20px;
  font-size: 14px;
  text-align: center;
}
</style>
