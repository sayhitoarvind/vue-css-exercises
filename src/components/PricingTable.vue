<template>
  <div class="cards grid grid-cols-3 gap-8">
    <FlexCard v-for="(info,index) in pricing" :title="info.title" :desc="info.desc" :key="index" />
  </div>
</template>

<script>
import FlexCard from '@/components/FlexCard.vue'

export default {
  name: 'PricingTable',
  components: {
    FlexCard
  },
  data() {
    return {
      pricing: [{
        title: 'Basic',
        desc: `500GB Storage. \n Maximum 2 users allowed. \n send up to 3GB`
      },
      {
        title: 'Professional',
        desc: `1TB Storage. \n Maximum 10 users allowed. \n send up to 20GB`
      },
      {
        title: 'Enterprise',
        desc: `2TB Storage. \n Maximum 50 users allowed. \n send up to 1000GB`
      }
      ]
    }
  }

}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="sass" scoped>
.cards 
  display: flex
  align-items: stretch
  justify-content: center
  margin-top: 160px
</style>
