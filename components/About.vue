<template>
  <section class="about-section">
    <div class="container">
      <div class="row">
        <div class="col-lg-6 col-sm-12 col-xs-12">
          <div class="about-image">
            <img :src="require('static/img/watch-02.jpg')" alt="about-image" />
          </div>
        </div>
      </div>
    </div>
  </section>
</template>
<style>
.about-section {
  padding: 100px;
}
.about-section .about-image img {
  max-width: 450px;
  width: 100%;
}
.about-section .about-image {
  margin: auto;
}
</style>
