<template>
  <header class="header fixed-top">
    <div class="container">
      <nav class="navbar navbar-expand-md navbar-light">
        <!-- Brand -->
        <a class="navbar-brand" href="#">VueShop</a>

        <!-- Toggler/collapsibe Button -->
        <button
          class="navbar-toggler"
          type="button"
          data-toggle="collapse"
          data-target="#collapsibleNavbar"
        >
          <span class="navbar-toggler-icon"></span>
        </button>

        <!-- Navbar links -->
        <div id="collapsibleNavbar" class="collapse navbar-collapse">
          <ul class="navbar-nav ml-auto">
            <li class="nav-item">
              <a class="nav-link active" href="#">Home</a>
            </li>
            <li class="nav-item">
              <a class="nav-link" href="#">About</a>
            </li>
            <li class="nav-item">
              <a class="nav-link" href="#">Features</a>
            </li>
            <li class="nav-item">
              <a class="nav-link" href="#">Products</a>
            </li>
            <li class="nav-item">
              <a class="nav-link" href="#">Testimonial</a>
            </li>
            <li class="nav-item">
              <a class="nav-link" href="#">Contact</a>
            </li>
          </ul>
        </div>
      </nav>
    </div>
  </header>
</template>
<style scoped>
.header .navbar {
  padding: 0;
}
.header {
  border: 1px solid rgba(255, 255, 255, 0.2);
}
.header .navbar .navbar-brand {
  font-size: 30px;
  color: #ffffff;
  font-weight: 700;
}
.header .navbar #collapsibleNavbar .nav-item .nav-link {
  color: white;
  font-size: 16px;
  font-weight: 600;
  padding: 20px 15px 20px;
  line-height: 26px;
  opacity: 0.6;
}

.header .navbar #collapsibleNavbar .nav-item .active {
  opacity: 1;
}
</style>
