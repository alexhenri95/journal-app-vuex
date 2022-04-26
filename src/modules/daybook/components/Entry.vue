<template>
    <div class="entry-container pointer p-2" @click="$router.push({name: 'entry', params: {id: 10}})">
        <!-- titulo -->
        <div class="entry-title d-flex">
            <span class="text-success fs-5 fw-bold">24</span>
            <span class="mx-1 fs-5"> Abril</span>
            <span class="mx-2 fw-light"> 2021, domingo</span>
        </div>

        <div class="entry-description">
            <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Laborum sit laudantium, incidunt fuga error ad nobis quia cupiditate magni enim, architecto vel facere inventore dolor est. Nihil itaque nam quisquam.</p>
        </div>
    </div>
</template>

<style lang="scss" scoped>
.entry-container {
    border-bottom: 1px solid #2c3e50;
    transition: 0.2s all ease-in;

    &:hover {
        background-color: lighten($color: grey, $amount: 45);
    }

    .entry-description p {
        font-size: 14px;
    }
}
</style>