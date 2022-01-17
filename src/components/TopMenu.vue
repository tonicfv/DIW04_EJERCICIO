<template>
  <div class="top_menu">
    <div class="buscar">
         
        <form class="form-search">
          <div class="input-group">
            <input class="form-control form-text" maxlength="128" placeholder="Buscar" size="15" type="text" />
            <span class="input-group-btn"><button class="btn btn-primary"><i class="fa fa-search fa-lg">&nbsp;</i></button></span>
          </div>
        </form>
  
    </div>

    <div class="top_menu_link">
    
        <a href="#">Mi Cuenta <i class="fas fa-user"></i></a>
       
        <a href="#">Cesta <i class="fas fa-shopping-cart"></i></a>

    </div>
  </div>
  
</template>

<script>
export default {};
</script>

<style>
.top_menu {
  display: flex;
  flex-direction: row;
  flex-grow: 1;
  align-items: center;
  justify-content: space-between;
  min-height: 60px;
  background-color: #ececed;
}
.top_menu_link  {
  margin-right: 1.5em;
  display: flex;
  flex-direction: row;
}
.top_menu_link a {
  margin-left: 15px;
  padding-left: 8px;

}

.top_menu a {
  color: rgb(3, 3, 3);
  margin-left: 5px;
  text-decoration: none;
}
.top_menu a:hover {
  color: rgb(255, 17, 0);
  margin-left: 5px;
  text-decoration: none;
}

.placeholder {
  font-family: "Font Awesome 5 Free";
  font-weight: 900;
  text-transform: uppercase;
}
.buscar {
  display: flex;
  flex-direction: row;
  flex-grow: 1;
  margin-left: 50px;
}
div input {
  width: 160px;
}

</style>