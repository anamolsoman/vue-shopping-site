<template>
  <section class="home-section primary">
    <v-container>
      <v-row justify="center">
        <v-col md="4" lg="4" cols="12" order-md="2" order-lg="2">
          <div class="home-img">
            <img :src="require('@/static/img/watch-01.png')" />
          </div>
        </v-col>
        <v-col md="4" lg="4" cols="12" order-md="1" order-lg="1">
          <div class="home-content">
            <h1>Present your awesome product</h1>
            <p>
              Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do
              eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut
              enim ad minim veniam, quis nostrud exercitation ullamco laboris
              nisi ut aliquip ex ea commodo consequat.
            </p>
            <a href="#" class="btn mybtn1">Buy For $150</a>
          </div>
        </v-col>
      </v-row>
    </v-container>
  </section>
</template>
<style>
.home-section {
  padding: 150px 0px 150px;
}
.home-section h1 {
  color: white;
  font-weight: 700;
  font-size: 55px;
  margin: 0;
  line-height: 60px;
}
.home-section p {
  color: white;
  font-size: 18px;
  margin-top: 20px;
  margin-bottom: 30px;
  line-height: 28px;
}
.home-section .btn {
  background-color: white;
  border-radius: 30px;
  font-size: 16px;
  font-weight: 600;
  text-transform: uppercase;
  padding: 12px 30px;
}
.home-section .btn:hover {
  background-color: black;
  color: white;
}
/* .home-section .home-img {
  position: relative;
} */
.home-section .home-img img {
  width: 100%;
  max-width: 400px;
  left: 150px;
  /* position: absolute; */
  top: -50px;
  margin: auto;
  animation: productani01 5s linear infinite;
}
.home-img {
  display: flex;
}
@keyframes productani01 {
  0%,
  100% {
    transform: translateY(15px);
  }
  50% {
    transform: translateY(-15px);
  }
}
</style>
