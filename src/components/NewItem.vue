<template>
  <div>
    <button @click="sayHello">Click me</button>
    <h1>Web development is my passion</h1>
    <p>{{mostacho}}</p>
    <a :href="link" target="_blank">my link</a>
    <img :src="imageSrc" alt="">
    <label for="name">Enter your name</label>
    <input id="name" type="text" v-model="yourName">
    <p>Hello {{yourName}}</p>
    <button @click="thanks"> Click if you like cats</button>
    <p>{{res}}</p>
    </div>
</template>

<script>
export default {
    data() {
        return {
            mostacho: "Es mi primerito día",
            link: "https://katenokk.github.io/mid-term-project/",
            imageSrc: "https://upload.wikimedia.org/wikipedia/commons/c/c7/Tabby_cat_with_blue_eyes-3336579.jpg",
            yourName: "",
        };
    },

    methods: {
        sayHello() {
            console.log("Hello");
        },
        thanks() {
            res: "Thank you!" //no funciona así?
        }
    }

}
</script>

<style>

img {
    width: 200px;
    display: block;
    margin: 0 auto;
}

</style>