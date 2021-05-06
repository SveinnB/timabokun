<template>
  <v-container>
    <Barcode :code="params.code" format="code128"/>
  </v-container>
</template>

<script>
import Barcode from '~/components/Barcode.vue'

export default {
  name: "BarcodePage",
  components: {
    Barcode
  },
  head(){
    return {
      title: 'Tímabókun'
    }
  },
  async asyncData({ params }) {
    return { params }
  }
}
</script>
