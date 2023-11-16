<template>
    <button :style="{backgroundColor: btnbgcolor}">
    </button>
</template>

<script>
export default{
    name: "Button",
    props: {
        btntext: String,
        btnbgcolor: String,
        
    }
}
</script>

<style>
    button{
        width: 120px;
        height: 40px;
        border-radius: 3px;
        border: none;
        
    }
</style>