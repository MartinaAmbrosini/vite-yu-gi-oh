<script >
export default {
    name: 'SingleItem',
    props: {
        info: Object
    }
}
</script>

<template>
    <div class="img-container">
        <img :src="info.card_images[0].image_url" :alt="info.name">
    </div>
    <div class="card-title">{{ info.name }}</div>
    <div class="card-type">{{ info.archetype }}</div>
</template>

<style lang="scss" scoped>
.img-container {
    width: 100%;

    img {
        width: 100%;
    }
}

.card-title {
    color: white;
    text-align: center;
    font-size: 20px;
    margin: 10px 0;
}

.card-type {
    text-align: center;
    font-size: 16px;
    margin-bottom: 6px;
}
</style>