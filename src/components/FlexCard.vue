<template>
  <div class="">
    <div class="card shadow-lg">
    <div class="card-title"> {{ title }} </div>
      <div class="card-image"> <img  src="@/assets/logo.png"> </div>
    <div class="card-description"> <pre> {{ desc }} </pre> </div>
    <button class="btn mb-2"> Learn more </button>
    </div>
  </div>
</template>

<script>
export default {
  name: 'FlexCard',
  props: {
    title: {
      default: () => 'title',
      type: String
    },
    desc: {
      default: () => 'Description',
      type: String
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="sass" scoped>
.card 
  border-radius: 6px

.card-title 
  display: flex
  justify-content: center
  color: #FFFFFF
  background-color: #C0C0C0

.card-image 
  display: flex
  max-width: 100%
  justify-content: center

.card-description
  display: flex
  justify-content: center
  text-align: center

.btn 
  color: #FFFFFF
  background-color: #2196F3
  border-radius: 5px
  text-align: center
  padding: 12px 16px
  font-size: 16px

  &:hover
    background-color: #448AFF

</style>
