<template>
   
    <section id="pie">
        <div class="made">
            <p> Made with Vue.js, Font Awesome, Materialize </p>
            <span class="terms">Terms Privacy </span>
             <a href="#"><span class="rs"><i class="fad fab fa-vuejs fa-2x" style="color: mediumseagreen;"></i></span></a>
             <a href="#"><span class="rs"><i class="fad fab fa-html5 fa-2x" style="color: orangered;"></i></span></a>
             <a href="#"><span class="rs"><i class="fad fab fa-css3 fa-2x" style="color: dodgerblue;"></i></span></a>
            <a href="#"><span class="rs"><i class="fad fab fa-font-awesome-flag fa-2x" style="color: deepskyblue;"></i></span></a>
 
                    
        </div>
        <div class="contacto">
            <h6>Ponte en contacto con nosotros</h6>
                <div class="contact">
                    <address>
                    EntuKeo Creative <br>
                    PO Box 4566, Mountain View, CA 
                    </address>

                    <ul class="menu">
                        <li><a href="mailto:info@entukeo.org" class="mail">info@entukeo.org</a></li>
                        <li><a href="https://entukeo.org/faq">Preguntas Frecuentes</a></li>
                    </ul>
                    <div class="menu-footer">
                        <ul class="menu">
                            <li  class="menu-item"><a href="#">Contacto</a></li>
                            <li  class="menu-item"><a href="#">Privacidad</a></li>
                            <li  class="menu-item"><a href="#">Politicas</a></li>
                            <li  class="menu-item"><a href="#">Términos</a></li>
                        </ul>
                    </div>
            </div>
            <a href="#"><span class="rs"><i class="fad fab fa-creative-commons-by" style="color: white;"></i></span></a>
            <a href="#"><span class="rs"><i class="fad fab fa-creative-commons" style="color: white;"></i></span></a>
        </div>
        <div id="rrss">
            <p>Siguenos en nuestras Redes Sociales</p>
            <a href="#"><span class="rs"><i class="fad fab fa-facebook fa-2x" style="color: white;"></i></span></a>
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
    height: 210px;
    padding-top:1rem;
    align-items: space-around;
    justify-content: space-between;
}
#pie span {
    margin: 8px;
}
#pie p {
    color:white;
    padding-bottom: 1px;
}
#pie a {
    color: whitesmoke;
}

#pie a:hover {
    color: rgb(255, 38, 0);
}
#rrss {
    color: whitesmoke;
    margin-top:20px;
    margin-right: 20px;
}

.contacto {
    margin:0 20px;
}

.contacto h6{
    font-size: 1.1em;
    color:white;
    margin:0;
    padding:10px;
}

.made {
    font-size: small;
    margin-top:26px;
    margin-left: 20px;
}
.menu {
    list-style: none;
    margin:0 auto;
    padding: 6px;
    text-align: left;
}

address {

    color: #999;
    font-size: 0.8rem;
    display: block;
    font-weight: 600;
    font-style: normal;
    margin:3px 2px;
}
.contact {
    display: flex;
    flex-direction: column;
}
.menu-footer {
    flex-direction: row;
    display: flex;
}
.menu-footer ul {
    text-align: left;
    margin: 1px 0;
 
}
.menu-footer li {
    color: #606060;
    margin-bottom: .5em;
    margin-right: 10px;
    padding-right: 10px;
    border-right: 1px solid #606060;
    display: inline;
    font-size: 0.8em;
    line-height: 0.9em;
    list-style: none;

}
.menu-footer li a {
    color: #8a8888 !important;
    text-decoration: none;

}
.terms {
margin:0 10px;
display:block;
padding: 10px;;
}


</style>