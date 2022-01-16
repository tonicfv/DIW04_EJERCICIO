<template>
   
    <section id="pie">
        <div class="contacto made">
            <p> Made with Vue.js, © Fonticons, 
            <br>Materialize Terms Privacy </p>
        </div>
        <div class="contacto">
            <p> <a href="#">Ponte en contacto con nosotros</a></p>
        </div>
        <div id="rrss">
            <p>Siguenos en nuestras Redes Sociales</p>
            <a href="#"><span class="rs"><i class="fad fab fa-facebook  fa-2x" style="color: white;"></i></span></a>
            <a href="#"><span class="rs"><i class="fad fab fa-twitter-square fa-2x" style="color: white;"></i></span></a>
            <a href="#"><span class="rs"><i class="fad fab fa-instagram fa-2x" style="color: white;"></i></span></a>
        </div>
    </section>

</template>

<script>
export default {


}
</script>

<style>

#pie{
    display:flex;
    background-color: rgb(38, 38, 38);
    height: 130px;
    padding-top:1rem;
    align-items: space-around;
    justify-content: space-between;
}
#pie span {
    margin: 8px;
}
#pie p {
    color:white;
}
#pie a {
    color: whitesmoke;
    
}

#pie a:hover {
    color: rgb(255, 38, 0);
}
#rrss {
    color: whitesmoke;
}

.contacto {
    margin:0 20px;
}
.made {
    font-size: small;
}



</style>