<template>
    <div class="main">
        <div class="card">
            <div class="contents">
                <img 
                :src="cartella.thumb" 
                :alt="cartella.titolo"
                >
                <h2> {{cartella.series}} </h2>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'CardDc',
    props: {
        cartella: Object,
    },
}
</script>

<style lang="scss" scoped>

.card {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    text-align: center;

    img {
        height: 100px;
    }

    .contents {
        // background-image: url(./img/favicon.ico);
        background-color: white;
        padding: 1em;
        width: 200px;
        color: black;
    }

    h2 {
        font-size: 12px;
    }
}

</style>