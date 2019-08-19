
<template>
  <v-container fluid fill-height>
    <v-layout align-center justify-center>
      <v-btn color="primary" @click="setLayout('simple-layout')">Simple Layout</v-btn>
      <v-btn color="secondary" @click="setLayout('app-layout')">App Layout</v-btn>
     <router-link to="/about">About</router-link>
    </v-layout>
  </v-container>
</template>

<script>
export default {
  mounted: function () {
   
      this.$store.commit('SET_LAYOUT','app-layout')
    
  },
  methods: {
    setLayout (layout) {
      this.$store.commit('SET_LAYOUT', layout)
    }
  }
}
</script>
