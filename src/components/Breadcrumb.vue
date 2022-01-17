<template>

 <ul id="breadcrumbs-one">
  <li><a href="#"><i class="fas fa-home"></i></a></li>
  <li><a href="#">Decoracion</a></li>
  <li><a href="#">Interior</a></li>
  <li><a href="#">Salón</a></li>
  <li><a href="#" id="activeitem">Sillas</a></li>
  
</ul>

</template>

<script>
export default {

}
</script>

<style>
#breadcrumbs-one{
  display: flex;
    align-content: center;
    justify-content: center;
    overflow: hidden;
    width: 100%;
  }

  #breadcrumbs-one li{
    float: left;
    list-style: none;
  }

  #breadcrumbs-one a{
    padding: .1em 1em .1em 2em;
    float: left;
    text-decoration: none;
    color: #444;
    position: relative;
    text-shadow: 0 1px 0 rgba(255,255,255,.5);
    background-color: #ddd;
    background-image: linear-gradient(to right, #f5f5f5, rgb(238, 236, 236));
  }

  #breadcrumbs-one li:first-child a{
    padding-left: 1em;
    border-radius: 5px 0 0 5px;
  }

  #breadcrumbs-one a:hover{
    background: #fff;
  }

  #breadcrumbs-one a::after,
  #breadcrumbs-one a::before{
    content: "";
    position: absolute;
    top: 50%;
    margin-top: -1.5em;
    border-top: 1.5em solid transparent;
    border-bottom: 1.5em solid transparent;
    border-left: 1em solid;
    right: -1em;
  }

  #breadcrumbs-one a::after{
    z-index: 2;
    border-left-color: rgb(238, 236, 236);
  }

  #breadcrumbs-one a::before{
    border-left-color: rgb(255, 255, 255);
    right: -1.1em;
    z-index: 1;
  }

  #breadcrumbs-one a:hover::after{
    border-left-color: #fff;
  }

  #breadcrumbs-one .current,
  #breadcrumbs-one .current:hover{
    font-weight: bold;
    background: none;
  }

  #breadcrumbs-one .current::after,
  #breadcrumbs-one .current::before{
    content: normal;
  }
  #activeitem {
    color:rgb(248, 29, 4) !important;
  
  }
 
</style>