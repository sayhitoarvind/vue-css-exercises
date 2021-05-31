<template>
  <div class="about">
    <Profile />
  </div>
</template>


<script>
import Profile from '@/components/Profile.vue'

export default {
  name: 'About',
  components: {
    Profile
  }
}
</script>

<style lang="sass" scoped>
.about 
  display: flex
  flex: 3
  min-height: 80vh
  justify-content: center
  align-items: center
  background-color: hsla(218, 100%, 18%, 1)
</style>
