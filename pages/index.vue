<template>
  <div>
    <head>
      <link
        rel="stylesheet"
        href="https://maxcdn.bootstrapcdn.com/bootstrap/4.5.2/css/bootstrap.min.css"
      />
      <!-- <link rel="stylesheet" href="../style/responsive.css" /> -->
      <script src="https://ajax.googleapis.com/ajax/libs/jquery/3.5.1/jquery.min.js"></script>
      <script src="https://cdnjs.cloudflare.com/ajax/libs/popper.js/1.16.0/umd/popper.min.js"></script>
      <script src="https://maxcdn.bootstrapcdn.com/bootstrap/4.5.2/js/bootstrap.min.js"></script>
    </head>
    <Header />
    <Home />
  </div>
</template>

<script>
export default {}
</script>
<style>
@import '../style/responsive.css';
@import url('https://fonts.googleapis.com/css2?family=Montserrat:wght@400;500;600;700;800;900&display=swap');
body {
  margin: 0;
  font-size: 16px;
  font-family: 'Montserrat', sans-serif;
  font-weight: 400;
}
* {
  margin: 0;
  padding: 0;
  outline: none;
}
a {
  text-decoration: none !important;
}
.header,
.home-section {
  background-color: #d70d25;
}
</style>
