<template>
  <div> {{SomeData}} {{Today }}</div>
</template>

<script>
export default {
    name: 'Main',
    data(){
        return{
            SomeData: 'Some random data',
            Today: Date()
        }
    }

}
</script>

<style>

</style>