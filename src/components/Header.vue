<template>
  <div>{{ header }}</div>
  <div>The year is {{ todaysDate }}</div>
  <button v-on:click="showDate">Click to show date</button>
  <p>{{computedTime}}</p>
</template>

<script>
export default {
    name: 'header',
    data() {
      return {
        header: 'The header',
        todaysDate: null,
        computedTime: null
      }
        
    },
    methods: {
        showDate(){
        let today = new Date()
        console.log(today)
        this.todaysDate = today.getFullYear()

        console.log(this.todaysDate)
      }
    },
    computed: {
      computedFunction(){
         this.computedTime = new Date()
         console.log('this is'+this.computedTime)
         return this.computedTime
      }
      
    }
    

}
</script>

<style>

</style>