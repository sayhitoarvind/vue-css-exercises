<template>
  <div class="card shadow-lg">
      <div class="avatar mt-14">
<img class="inline object-cover w-16 h-16 mr-2 rounded-full" src="https://images.pexels.com/photos/2589653/pexels-photo-2589653.jpeg?auto=compress&cs=tinysrgb&h=650&w=940" alt="Profile image"/>
       </div>
 <div class="title">
  <div class="mx-1 name"> Victor Stone </div>
   <div class="mx-1 age"> 28 </div> 
 </div>
  <div class="location"> Ontario </div>
  <div class="divider" />
  <div class="socialmedia">
 <div> 80K <div class="socialmedia__small"> Followers </div> </div> <div > 800K <div class="socialmedia__small" > Likes </div> </div> <div> 2.4K <div class="socialmedia__small"> Posts </div> </div> 
 </div>
  </div>
</template>

<script>
export default {
  name: 'Profile',
  props: {

  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="sass" scoped>
.card   
    border-radius: 20px
    display: flex
    flex-direction: column
    height: 280px
    width: 300px
    background-color: #FFFFFF
    
.title
    display: flex
    justify-content: center 

.name 
    font-size: 22px
    font-weight: bold

.age 
    color: grey
    font-size: 22px
    font-weight: bold

.location
    color: grey
    display: flex
    flex: 3
    justify-content: center
    font-weight: bold

.socialmedia
    display: flex
    flex: 1
    justify-content: space-around
    font-size: 22px
    font-weight: bold

.socialmedia__small
    color: grey
    font-size: 12px

.divider 
    border-top: 1px solid #bbb
    padding-top: 1em

</style>
