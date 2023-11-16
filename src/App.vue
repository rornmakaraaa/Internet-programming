<template>
  <div class="wrapper">
    <Category v-for="i in Category" 
            :key="i.Category"
            :bgcolor="i.bgcolor" 
            :image="i.image" 
            :Product="i.Product"
            :quantity="i.quantity"></Category>
</div>
  <br>

  <div class="promotion-container">
    <Promotion v-for="i in Promotion" :key="i.Promotion"
            :colorBackground="i.colorBackground" 
            :description="i.description"
            :productImages="i.productImages"
            :btnbgcolor="i.btnbgcolor"
            :btntext="i.btntext">

    </Promotion>
  </div>
  <br>
  </template>

<script>
import Category from "./components/Category.vue";
import Button from "./components/Button.vue";
import Promotion from "./components/Promotion.vue";

export default{
  name: "App",
  components:{
    Category,
    Button,
    Promotion,
    
  },

  data(){
    return{
      Category: [
        {
          bgcolor: "#F2FCE4",
          image: "https://www.figma.com/file/365MrAv8OiWgwbDhMr0jAJ/image/8370e9158a586f746c0b10b70cd405c8aa1f2038",
          Product: "Cake & Milk",
          quantity: "14 items"
        },
        {
          bgcolor: "#FFFCEB",
          image: "https://www.figma.com/file/365MrAv8OiWgwbDhMr0jAJ/image/fa196bce6720167ebdfcf5d3f8a2d76053176f9a",
          Product: "Peach",
          quantity: "17 items"
        },
        {
          bgcolor: "#ECFFEC",
          image: "https://www.figma.com/file/365MrAv8OiWgwbDhMr0jAJ/image/eb0a46d6bf3d30616b8cd69f4b03064fe254350c",
          Product: "Oganic Kiwi",
          quantity: "21 items"
        },
        {
          bgcolor: "#FEEFEA",
          image: "https://www.figma.com/file/365MrAv8OiWgwbDhMr0jAJ/image/21b63a1ef2a493eea176934bcab372692ab59a29",
          Product: "Red Apple",
          quantity: "68 items"
        },
        {
          bgcolor: "#FFF3EB",
          image: "https://www.figma.com/file/365MrAv8OiWgwbDhMr0jAJ/image/488cb40d98f6efd89c2347f8ab7f23b7757a7e2f",
          Product: "Snack",
          quantity: "34 items"
        },
        {
          bgcolor: "#FFF3FF",
          image: "https://www.figma.com/file/365MrAv8OiWgwbDhMr0jAJ/image/13f9afc802816b515e817bcd88800c49b947f860",
          Product: "Black plum",
          quantity: "25 items"
        },
        {
          bgcolor: "#F2FCE4",
          image: "https://www.figma.com/file/365MrAv8OiWgwbDhMr0jAJ/image/5e6d35bccc6f73e5412576546dca6b013f4fc9c7",
          Product: "Vegetables",
          quantity: "65 items"
        },
        {
          bgcolor: "#FFFCEB",
          image: "https://www.figma.com/file/365MrAv8OiWgwbDhMr0jAJ/image/0ed944fa3bcccc269ae2cadb2fb25ac9b02ea29e",
          Product: "Headphone",
          quantity: "33 items"
        },
        {
          bgcolor: "#F2FCE4",
          image: "https://www.figma.com/file/365MrAv8OiWgwbDhMr0jAJ/image/78c48886688817c7c490b88407c4904743141184",
          Product: "Cake & Milk",
          quantity: "54 items"
        }, {
          bgcolor: "#FFF3FF",
          image: "https://www.figma.com/file/365MrAv8OiWgwbDhMr0jAJ/image/aadca20d2ca905cbdfec3bf306fbe70e1ca34a8a",
          Product: "Orange",
          quantity: "63 items"
        },
      ],

      Promotion: [
        {
          colorBackground: "#F0E8D5",
          productImages: "https://www.figma.com/file/365MrAv8OiWgwbDhMr0jAJ/image/de8c488a87b9ce16acd7436a6dec758331c840bc",  
          description: "Everyday Fresh & Clean with Our Products",
          btnbgcolor: "#3BB77E",
          btntext: "Shop now",
        },
        {
          colorBackground: "#F3E8E8",
          productImages: "https://www.figma.com/file/365MrAv8OiWgwbDhMr0jAJ/image/2738f29f1c4542246febe8c91ddb74ce42b81c5d",  
          description: "Make your Breakfast Healthy and Easy",
          btnbgcolor: "#3BB77E",
          btntext: "Shop now",
        },
        {
          colorBackground: "#E7EAF3",
          productImages: "https://www.figma.com/file/365MrAv8OiWgwbDhMr0jAJ/image/4d6961518879bc373bf5fcc1578bcec5172b087b",  
          description: "The best Organic Products Online",
          btnbgcolor: "#FDC040",
          btntext: "Shop now",
        },

      ]
    }
  },
}

</script>

<style scoped>
@import "https://unicons.iconscout.com/release/v4.0.0/css/line.css";
.wrapper{
  display: flex;
  justify-content: center;
  align-items: center;
  padding: 2px;
  gap: 10px;
}
.promotion-container{
  display: flex;
  justify-content: center;
  padding: 2px;
  gap: 20px;
}
</style>