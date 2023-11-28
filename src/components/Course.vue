<template>
    <div class="card shadow" style="margin-top: 20px;">
        <img :src="imgSrc" class="card-img-top" alt="...">
        <div class="card-body">
            <h5 class="card-title">{{courseName}}</h5>
            <p class="card-text">Some quick example text to build on the card title and make up the bulk of the card's content.</p>
            <a href="#" class="btn btn-primary">Go somewhere</a>
        </div>
    </div>
</template>

<script>
    export default{
        props:["imgSrc","courseName"]
    }
</script>

<style>

</style>