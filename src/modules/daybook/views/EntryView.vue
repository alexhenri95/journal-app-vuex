<template>
    <div class="entry-title d-flex justify-content-between p-2">
        <div>
            <span class="text-success fs-3 fw-bold">24</span>
            <span class="mx-1 fs-3">Abril</span>
            <span class="mx-2 fs-4 fw-light">2022, domingo</span>
        </div>

        <div>
            <button class="btn btn-danger mx-2">
                Borrar
                <i class="fa fa-trash-alt"></i>
            </button>

            <button class="btn btn-primary">
                Borrar
                <i class="fa fa-upload"></i>
            </button>
        </div>
    </div>

    <hr>

    <div class="d-flex flex-column px-3 h-75">
        <textarea placeholder="¿Que sucedió hoy?"></textarea>
    </div>

    <Fab icon="fa-save"/>

    <img src="https://definicion.de/wp-content/uploads/2009/12/paisaje-1.jpg" class="img-thumbnail" alt="">

</template>

<script>
import { defineAsyncComponent } from 'vue'
export default {
    components: {
        Fab: defineAsyncComponent( () => import('../components/Fab'))
    }
}
</script>

<style lang="scss" scoped>
textarea {
    font-size: 20px;
    border: none;
    height: 100%;

    &:focus {
        outline: none;
    }
}

img {
    width: 200px;
    position: fixed;
    bottom: 120px;
    right: 20px;
    box-shadow: 0px 5px 10px rgba($color: black, $alpha: 0.7);
}
</style>