<template>
  <v-content>
    <v-layout
      row
      class="head">
      <v-flex>
        <v-layout
          class="red"
          justify-center
          row
          align-center
          fill-height>
          <tiletitle/>
          <subtitle/>
        </v-layout>
        <v-layout
          row>
          <v-flex
            xs12
            sm5
            md5>
            <v-tabs
              v-model="headtab"
              color="lighten-4 blue">
              <v-tab
                v-for="n in optionsHead"
                :key="n.length">
                {{ n.title }}
              </v-tab>
            </v-tabs>
          </v-flex>
          <v-flex
            xs12
            sm5
            md5
            offset-xs0
            offset-lg2>
            Founders
          </v-flex>
        </v-layout>
      </v-flex>
    </v-layout>
  </v-content>
</template>
<script>
import subtitle from '@/components/index/tagline/subview'
import tiletitle from '@/components/index/tagline/titleview'
export default {
  components: {
    subtitle,
    tiletitle
  },
  data() {
    return {
      headtab: null,
      optionsHead: [
        { title: 'Home', icon: 'dashboard' },
        { title: 'About', icon: 'dashboard' }
      ]
    }
  }
}
</script>
<style scoped>
.head {
  height: 300px;
}
</style>
