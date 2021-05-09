<template>
  <div>
    <Hero />
    <LargeCardDisplay class="large-card-sec"
      v-for="cardInfo in LargeCardInfo"
      :key="cardInfo.id"
      :cardSection="cardInfo"
     />
  </div>
</template>

<script>
import { largeCardSections } from '@/assets/data.js'
export default {
  data(){
    return {
      LargeCardInfo: largeCardSections
    }
  }
}
</script>

<style>

</style>
