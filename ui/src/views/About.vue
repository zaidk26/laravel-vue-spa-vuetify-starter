<template>
  <v-container fluid fill-height>
   <h1>Test</h1>
  </v-container>
</template>

<script>
export default {
  mounted: function () {
   
      this.$store.commit('SET_LAYOUT','simple-layout')
    
  }
}
</script>