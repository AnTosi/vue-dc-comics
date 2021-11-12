<template>
    <div class="card col-16 mb-4">
        <img :src="thumb" alt="">
        <h3>{{series.toUpperCase()}}</h3>
    </div>
</template>

<script>
export default {
    props: {
        thumb: String,
        series: String
    }
}
</script>

<style lang="scss">
    .card {
        h3 {
            font-size: 0.7rem;
            font-weight: 400;
            margin-top: 0.3rem;
        }
    
        img {
            width: 185px;
            height: 185px;
            object-fit: cover;
            object-position: top;
        }
    }
</style>