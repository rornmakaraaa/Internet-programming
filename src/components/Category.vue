<template>
    <div class="container" :style="{ backgroundColor : bgcolor}">
        <img :src="image" alt="burger">
        <h3>{{Product}}</h3>
        <p>{{quantity}}</p>
    </div>
</template>

<script>
export default{
    name: "Category",
    props: ["bgcolor", "image", "Product", "quantity"]
}
</script>

<style scoped>
@import "https://unicons.iconscout.com/release/v4.0.0/css/line.css";
    .container{
        width: 148px;
        height: 177px;
        border-radius: 10px;
        background: #F2FCE4;
        box-shadow: 20px 20px 40px 0px rgba(24, 24, 24, 0.07);
    }
    img{
        margin: 0 0 -15px 0;
        width: 120px;
        height: 120px;
        flex-shrink: 0;
        


    }
    h3 ,p{
        color: var(--NestMart-TextHeading, #253D4E);
        text-align: center;
        font-family: Quicksand;
        font-size: 16px;
        font-weight: 700;
    }
    p{
        color: var(--NestMart-Text-Muted, #b6b6b6);
        text-align: center;
        font-family: Lato;
        font-size: 12px;
        font-style: normal;
        font-weight: 400;
        line-height: 18px;
    }
    
</style>