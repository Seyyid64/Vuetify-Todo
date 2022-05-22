<template>
    <v-btn class="button-done-sorting" @click="$store.commit('toggleSorting')" color="primary">
        Done Sorting
    </v-btn>
</template>

<script>
export default {

}
</script>

<style>
.button-done-sorting {
    position: fixed;
    left: 50%;
    transform: translateX(-50%);
    bottom: 20px;
}
</style>