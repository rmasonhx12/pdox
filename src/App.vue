<template>
  <!-- Clean up initial app for dev -->
  <div id="app">
    <Docs v-bind:items="items"/>
    

    
  </div>
</template>

<script>
  import Docs from './components/Docs.vue'
export default {
  name: 'App',
  components: {
    Docs
  },
  // define our data
  data: () => {
    return {
      items: [
        {
          id: 1,
          name: "Test 1",
          exp: "16 Oct 2019"
        },
        {
          id: 2,
          name: "Test 2",
          exp: "19 Oct 2020"
        },
        {
          id: 3,
          name: "Test 3",
          exp: "14 Oct 2021"
        },
      ]
    }
  }
}
</script>

<style>

</style>
