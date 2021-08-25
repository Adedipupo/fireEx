<template>
    <div>
        <h1>{{product}} </h1>
    </div>
</template>

<script>
    export default {
        computed: {
            product(){
                return this.$store.getters.getProductById(this.$route.params.id)
            }
        }
    }
</script>

<style  scoped>

</style>