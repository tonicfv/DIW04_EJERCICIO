<template>
  <div class="content-main">
    <div class="header">
      <div class="top_menu"><TopMenu /></div>
      <div><Header /></div>
      <div class="main_menu"><MainMenu /></div>
      <div class="breadcrumb"><Breadcrumb /></div>
    </div>
    <div class="dos_columnas">
        <ProductoImagen/>
          <Images />
        <div class="rcolumn">
          <FichaProducto/>
        </div>
    </div>
    <div class="footer">
      <Pie />
    </div>
  </div>

</template>

<script>
import Header from "./components/Header.vue";
import MainMenu from "./components/MainMenu.vue";
import TopMenu from "./components/TopMenu.vue";
import Breadcrumb from "./components/Breadcrumb.vue";
import Images from "./components/Images.vue";
import FichaProducto from "./components/FichaProducto.vue";
import Pie from "./components/Pie.vue";

export default {
  name: "App",
  components: {
    MainMenu,
    Header,
    TopMenu,
    Breadcrumb,
    Images,
    FichaProducto,
    Pie
  },
};
</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Source+Sans+Pro:wght@200&display=swap');
#app {
  padding: 0;
  box-sizing: border-box;
  font-family: 'Source Sans Pro', sans-serif;
  text-align: center;
  background-color: rgb(252, 252, 252);
  margin: 0 auto;
}
body {
  margin: 0px;
  padding: 0px;
  box-sizing: border-box;
  font-family: 'Source Sans Pro', sans-serif;
  color: #333;
  height: auto;
  min-height: 100%;
}
.content-main {
	margin:auto;
	/* Flexbox */
	display:flex;
	flex-flow:column wrap;
}



.dos_columnas {
  padding-top:4rem;
  display: flex;
  align-content: center;
  justify-content: space-around;
  flex-wrap:wrap;

}

.rcolumn {
    margin-right:50px;
    min-width: 450px;

}
</style>
