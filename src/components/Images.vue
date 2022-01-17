<template>
    <section id="imgMain">
        <div class="imgCtal">
            <img class="imgLarge" v-bind:src="photos[0]" alt="Silla Ahelie" copyright="cc-by El gato">
        </div>
        <div class="slide">
            <a @click="changeImg(1)"><img class="imgSmall" v-bind:src="photos[1]" alt="Silla Ahelie"> </a>
            <a @click="changeImg(2)"><img class="imgSmall" v-bind:src="photos[2]" alt="Silla Ahelie"></a>
            <a @click="changeImg(3)"><img class="imgSmall" v-bind:src="photos[3]" alt="Silla Ahelie"></a>
            <a @click="changeImg(4)"><img class="imgSmall" v-bind:src="photos[4]" alt="Silla Ahelie"></a>
        </div>
    </section>
</template>

<script>
export default {
    Name: 'imagen',
    data () {
        return {
            photos: [
                require ('../assets/s1.jpg'),
                require ('../assets/s2.jpg'),
                require ('../assets/s3.jpg'),
                require ('../assets/s4.jpg'),
                require ('../assets/s5.jpg'),
                ]
        }
    },
    methods: {
        changeImg(id) {
            this.photos[0] = this.photos[id]
        }
    }
}
</script>

<style>
#imgMain {
    display: flex;
    flex-direction: column;
    border:0;
    flex: 1;
}
.imgCtal {
    height: 600px;
}

.imgLarge {
    height: 90%;
}
.imgSmall {
        height: 100px;
        margin-left:0px;
}
.slide {
    display: flex;
    justify-content: center;
    flex-direction: row;
    padding: 20px;
}
</style>