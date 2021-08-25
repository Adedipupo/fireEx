<template>
  <div class="container">
    <Hero />
    <LargeCardDisplay
      v-for="cardInfo in largeCardInfo"
      :key="cardInfo.id"
      :cardsSection="cardInfo"
    />
    <SmallCardDisplay
     v-for="smallCardInfo in smallCardInfo"
     :key="smallCardInfo.id"
     :smallCardsSection="smallCardInfo"
     />
  </div>
</template>

<script>
import { largeCardSections } from "@/assets/data.js";
import { smallCardSections } from "@/assets/data.js";

export default {
  data() {
    return {
      largeCardInfo: largeCardSections,
      smallCardInfo: smallCardSections,
    };
  }
};
</script>
