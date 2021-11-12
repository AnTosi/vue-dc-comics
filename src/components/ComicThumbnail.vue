<template>
    <div class="card col-16 mb-4 d-flex flex-column align-items-center">
        <img :src="thumb" alt="">
        <div class="title_container">
            <h3 class="text-left">{{series.toUpperCase()}}</h3>
        </div>
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
            font-size: 0.75rem;
            font-weight: 400;
            margin-top: 0.75rem;
        }
    
        img {
            width: 185px;
            height: 185px;
            object-fit: cover;
            object-position: top;
        }

        .title_container {
            width: 185px;
            
        }
    }
</style>