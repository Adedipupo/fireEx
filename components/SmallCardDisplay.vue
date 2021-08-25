<template>
    <div class="container">
        <h3 class="header">{{smallCardsSection.title}}</h3>
        <div class="card-container">
            <SmallCard 
              v-for="card in smallCardsSection.cards"
              :key="card.id"
              :card="card"
            />
        </div>
    </div>
</template>

<script>
    export default {
        props: ['smallCardsSection']
    }
</script>

<style scoped>
    .container {
        padding: 2rem 0
    }
    .header {
        font-weight: 700;
        font-size: 1.5rem;
        margin-bottom: 2rem;
    }
    .card-container {
        display: flex;
        justify-content: space-between;
        flex-wrap: wrap;
    }
</style>