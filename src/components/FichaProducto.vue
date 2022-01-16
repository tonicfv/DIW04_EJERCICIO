<template>
    <section id="ficha_prod">
        <h1 class="titulo">SILLA AHELIE </h1>

        <p>Precio: <span class="precio">189,00 €</span></p>
        <p>Silla giratoria a 360º tapizada con patas en metal de color negro </p>
        <p>Medidas: 52 x 57,50 x 84 cm</p>
        <p>Plazo de entrega: 7 días</p>

        <form>
            <label for="cantidad">Cantidad:  </label>
            <button @click="cambiarContador('-1')" type="button" name="button">-</button>
            <input type="text" :value="contador" name="cantidad"/>
            <button @click="cambiarContador('1')" type="button" name="button">+</button>
        </form>

        <button class="button boton_compra">  AÑADIR A LA CESTA</button>
           <div class="video">
            <video width="420" controls preload="auto" >
             <source src="../assets/videoint.mp4" type="video/mp4" />
         </video>
     </div>

    </section>

</template>

<script>
export default {
    Name: 'FichaProducto',
    data () {
        return {
            contador: 1
        }
    },
    methods: {
        cambiarContador(num){
            this.contador += +num;
            if(!isNaN(this.contador) && (this.contador < 0)) {
                this.contador = 0
            }
        }
    }

}
</script>

<style>

#ficha_prod {
    border: 1px solid rgb(208, 206, 206);
    border-radius: 2%;
    height: 750px;
}

.titulo {
    font-size:2rem;
    color: #333;
    border-bottom: 1px solid grey;
}

p {
    margin: 10px;
    padding: 12px;
    text-align: left;
}

#ficha_prod .precio {
    font-weight: 600;
    font-size:1.4rem;
    color:#ff0040;
}

.boton_compra {
    margin:3em 0;
    padding: 10px;
    position: relative;
    display: block;
    border:none;
    width: 100%;
    cursor: pointer;
    background-color: rgb(175, 172, 172);
    letter-spacing: 3px;
    color: #ffffff;
    text-align: center;
    outline: none !important;
    font-family: 'HelveticaNeueLTStd-LtCn';
}

.button {
  transition-duration: 0.7s;
}
.button:hover {
  background-color: #0f0f0f;
  color: white;
}

#ficha_prod form input {
    width:2rem;
    text-align:center;
    border: 1px solid #070707;
    font-size: 1rem;
    height:2rem;
}

#ficha_prod form button {
    height:2.3rem;
    width:2rem;
    border: 1px solid #d8d8d8;
}

</style>