<template>
  <div class="body">
    <div class="header">收款帳戶</div>
    <ul>
      <li v-for="index in 4" :key="index">
        <div class="inout">
          <input type="radio">
        </div>
        <div>
          <h2>中國郵政銀行ＸＸ支行</h2>
          <h3>阿狸</h3>
          <h4>6217 8888 8888 9997 789</h4>
        </div>
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.body {
  background-color: rgb(247, 246, 251);
}
.header {
  text-align: center;
  background-color: white;
  padding: 5px 0;
  margin-bottom: 5px;
  color: black;
  font-size: 28px;
}
.header::before {
  content: " ";
  width: 10px;
  height: 10px;
  rotate: 45;
  border: 2px;
  border-color: black;
}
ul {
  margin: 0;
  padding: 0;
}
.input {
  padding: 78px 28px 0 30px;
}
input {
  margin-top: 78px;
}
li {
  background-color: white;
  display: flex;
  margin-bottom: 30px;
  text-align: left;
}
input {
  width: 42px;
  height: 42px;
}
h2 {
  color: rgb(170, 170, 170);
  font-size: 28px;
  margin-top: 42px 0 0 0;
  padding: 0;
}
h3 {
  margin: 28px 0 0 0;
  padding: 0;
  color: rgb(51, 51, 51);
  font-size: 28px;
}
h4 {
  margin: 10px 40px 0 0;
  padding: 0;
  color: rgb(51, 51, 51);
  font-size: 28px;
}
</style>
