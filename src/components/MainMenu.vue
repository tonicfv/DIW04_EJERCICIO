<template>
  <div class="main_menu">
    <div class="link">
      <a href="#">LIQUIDACIÓN</a>
      <a href="#">NOVEDADES</a>
      <a href="#">DECORACIÓN</a>
      <a href="#">JARDÍN</a>
      <a href="#">MOBILIARIO</a>
      <a href="#">LIFESTYLE</a>
      <a href="#">MARCAS</a>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style>
.link {
  display: flex;
  flex-direction: row;
  align-items: center;
  justify-content: space-around;
}
.link a {
  color: rgb(7, 7, 7);
  text-decoration: none;
  margin: 20px;
  align-items: center;
  font-size: 21px;
  font-family: "CenturyGothic" !important;
  font-weight: normal !important;
  letter-spacing: 1px;
}

.link_menu {
  display: flex;
  align-items: center;
}
.link a:hover {
  color: #eb2027;
  font-weight: bold;
}

.main_menu {
  display: flex;
  flex-direction: row;
  align-items: center;
  justify-content: center;
  height: 25px;
}
.main_menu a {
  margin: 10px;
}
</style>