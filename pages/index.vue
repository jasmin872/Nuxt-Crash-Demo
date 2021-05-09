<template>
  <div>
    <Nav />
    <Hero />
    <LargeCardDisplay
      v-for="cardInfo in LargeCardInfo"
      :key="cardInfo.id"
      :cardSection="cardInfo"
     />
     <SmallCardDisplay
     v-for="cardInfo in smallCardSections"
      :key="cardInfo.id"
      :cardSection="cardInfo"
      />
  </div>
</template>

<script>
import { largeCardSections, smallCardSections } from '@/assets/data.js'
export default {
  data(){
    return {
      LargeCardInfo: largeCardSections,
      smallCardSections,
    }
  }
}
</script>

<style>

</style>
