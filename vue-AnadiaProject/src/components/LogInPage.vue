<template>
  <div>
    <img class="logo" src="../assets/VetLogo/pawprint.png" />
    <h1>Sign Up</h1>
    <div class="register">
      <input type="text" placeholder="Enter Name" />
      <input type="text" placeholder="Enter Name" />
      <input type="text" placeholder="Enter Name" />
      <button>Sign Up</button>
    </div>
  </div>
</template>

<script>
// export default {
//   name: "LogInPage",
// };
</script>

<style scoped>
.logo {
  width: 100px;
}

.register input {
  width: 300px;
  height: 40px;
  padding-left: 20px;
  display: block;
  margin-bottom: 30px;
  margin-right: auto;
  margin-left: auto;
  border: 1px solid skyblue;
}

.register button {
  width: 320px;
  height: 40px;
  border: 1px solid skyblue;
  background: skyblue;
  color: #fff;
  cursor: pointer;
}
</style>
