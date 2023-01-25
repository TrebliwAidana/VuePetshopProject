<template>
  <div class="desktop-1screen">
    <div class="overlap-group2">
      <img class="image-home" src="Homepage/image-13.png" alt="image 13" />
      <div class="home">HOME</div>
      <img
        class="image-appointment"
        src="Homepage/image-12.png"
        alt="image 12"
      />
      <div class="appointment">
        APPOINTMENT
      </div>
      <div>
        <img class="image-login" src="Homepage/image-11.png" alt="image 11" />
        <div class="log-in" >LOG IN</div>
      </div>
    </div>
    <div class="overlap-group1">
      <img class="image-1" src="Homepage/image-1.png" alt="image 1" />
      <p>
        <div class="line1">
        Pawsitively Great Care.
      </div>
      </p>
      <p
        class="line2"
      >
        Providing Special Care For Your Pets.
      </p>
      <p class="line3">
        Your pets deserve the finest in veterinary care!
      </p>
      <div class="rectangle-title"></div>
      <h1 class="title">Aidana Veterinary Care</h1>
    </div>
  </div>
</template>

<script setup>
  
</script>

<style scoped>
@import url("https://fonts.googleapis.com/css?family=Montserrat:700,600");

.desktop-1screen {
  align-items: flex-start;
  /* background-color: #d0e61b40; */
  background-color: whitesmoke;
  border: 1px none;
  display: flex;
  flex-direction: column;
  height: 1240px;
  width: 1440px;
  /* height: 100%;
  width:100%; */
}

.overlap-group2 {
  align-items: center;
  background-color: #ffc527;
  display: flex;
  height: 70px;
  /* width: 1440px; */
  width: 100%;
}
.image-home {
  height: 35px;
  margin-bottom: 24px;
  margin-top: 17px;
  margin-left: 50px;
  object-fit: cover;
  width: 35px;
}
.image-appointment {
  height: 60px;
  padding-left: 58%;
  /* padding-right: 0; */
  margin-top: 1px;
  object-fit: cover;
  width: 50px;
}
.image-login {
  height: 50px;
  padding-left: 180px;
  margin-top: 5px;
  object-fit: cover;
  width: 50px;
}

.appointment {
  left: 75.5%;
  top: 35px;
  font-size: 18px;
  letter-spacing: 0;
  margin-bottom: 10px;
  line-height: 18px;
  position: absolute;
  white-space: nowrap;
}

.home {
  font-size: 18px;
  letter-spacing: 0;
  line-height: 18px;
  margin-bottom: 5px;
  white-space: nowrap;
}

.log-in {

  left: 93%;
  font-size: 18px;
  letter-spacing: 0;
  line-height: 18px;
  margin-bottom: 10px;
  position: absolute;
  top: 35px; 
  white-space: nowrap;
}

.overlap-group1 {
  height: 1092px;
  position: relative;
  width: 100%;
}

.image-1 {
  height: 1140px;
  left: 0;
  object-fit: cover;
  position: absolute;
  border-radius: 5px;
  top: 30px;
  width: 80%;
  margin-left: 10%;
}

.rectangle-title {
  background-color: #ffd700;
  border-radius: 5px;
  height: 80px;
  left: 0;
  position: absolute;
  top: 5px;
  /* width: 1440px; */
  width: 78%;
  margin-left: 11%;
}

.title {
  color: black;
  font-family: var(--font-family-montserrat);
  font-size: 36px;
  line-height: 18px;
  position: absolute;
  left: 35%;
  top: 10px;
}
.line1 {
  left: 175px;
  letter-spacing: 0;
  line-height: 18px;
  position: absolute;
  top: 400px;
  font-size: 30px;
  font-style: var(--font-family-montserrat);
}

.line2 {
  left: 175px;
  letter-spacing: 0;
  line-height: 18px;
  position: absolute;
  top: 425px;
  font-size: 30px;
  font-style: var(--font-family-montserrat);
}

.line3 {
  left: 175px;
  letter-spacing: 0;
  line-height: 18px;
  position: absolute;
  top: 475px;
  font-size: 30px;
  font-style: var(--font-family-montserrat);
}

:root {
  --black: rgba(0, 0, 0, 1);
  --mexican-red: rgba(165, 42, 42, 1);

  --font-size-s: 24px;
  --font-size-m: 36px;
  --font-size-l: 80px;

  --font-family-montserrat: "Montserrat";
}

</style>
