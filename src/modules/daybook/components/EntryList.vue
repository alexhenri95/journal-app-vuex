<template>
    <div class="entry-list-container">
        <div class="px-2 pt-2">
            <input 
                type="text"
                class="form-control"
                placeholder="Buscar entradas..."
            >
        </div>

        <div class="entry-scrollarea">
            <Entry 
                v-for="item in 20"
                :key="item"
            />
        </div>
    </div>
</template>

<script>
import { defineAsyncComponent } from 'vue'
export default {
    components: {
        Entry: defineAsyncComponent( () => import('./Entry') )
    }
}
</script>

<style lang="scss" scoped>

input {
    height: 50px;
}

.entry-list-container {
    border-right: 1px solid #2c3e50;
    height: calc( 100vh - 56px );
}

.entry-scrollarea {
    height: calc( 100vh - 125px );
    overflow: scroll;
    margin-top: 10px;
}
</style>