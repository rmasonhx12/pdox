<template>
  <div id="app">
    <v-app>
      <v-layout row>
        <v-flex xs12 sm6 offset-sm3>
          <v-card>
            <Docs :items="items"/>
            <v-card-text style="height: 100px; position:relative">
              <v-btn 
                  big 
                  color="green"
                  dark
                  absolute
                  bottom
                  right
                  fab
                >
                <v-icon>add</v-icon>
                </v-btn>
            </v-card-text>
          </v-card>
        </v-flex>
      </v-layout>
    </v-app>
  
  
  </div>     
</template>

<script>
import Docs from './components/Docs.vue'


export default {
  name: 'app',

  components: {
    Docs
  },

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
