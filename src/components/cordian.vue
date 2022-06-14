<template>
<div>
    <h1 class="head">FRUITS</h1>
    <button class="button" v-on:click="apple">Apple</button>

    <p v-if="show_apple">An apple is an edible fruit produced by an apple tree. Apple trees are cultivated worldwide and are the most widely grown species in the genus Malus. </p>
    <button class="button" v-on:click="orange">Orange</button>

    <p v-if="show_orange">An orange is a fruit of various citrus species in the family Rutaceae; it primarily refers to Citrus  sinensis, which is also called sweet orange, </p>
    <button class="button" v-on:click="starwberry">Strawberry</button>

    <p v-if="show_starwberry">A small juicy red fruit that has small brown seeds on its surface, or the plant with white flowers on which this fruit grows: fresh strawberries. I thought we'd have strawberries and cream for dessert. strawberry jam/ice cream/tart. </p>
</div>

</template>

<script>

export default{
    name: 'CordiAn',
    data(){
        return {
            show_apple:false,
            show_orange:false,
            show_starwberry:false

        }
    },methods:{
        apple(){
            this.show_apple =!this.show_apple
        },
        orange(){
            this.show_orange =!this.show_orange

        },starwberry(){
            this.show_starwberry =!this.show_starwberry
        }

    }
}
</script>

<style scoped>
 .head{
     font-family: Georgia, 'Times New Roman', Times, serif;
     color: blueviolet;
 }
 .button{
     background-color: rgb(215, 250, 242);
     width: 70%;
     height: 50px;
 }

 p{
     width: 70%;
     height: 50px;
     margin-left: 189px;
    
 }
</style>