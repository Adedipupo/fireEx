<template>
    <div>
        <h1>{{products}}} </h1>
    </div>
</template>

<script>
import {mapState} from 'vuex'
    export default {
        computed:{
            ...mapState([
                'products'
            ])
        }
    }
</script>

<style  scoped>

</style>