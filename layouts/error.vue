<template>
  <v-container class="d-flex mt-10">
    <div class=" ma-auto d-flex flex-column justify-center">

      <template v-if="error.statusCode === 404">
        <v-img :src="require(`~/assets/404.png`)" alt="404 logo"
          contain
          class="ma-6"
          :max-height="700"
          :max-width="700">
        </v-img>
      </template>

      <template v-else>
        <h2 class="ma-3 text-h6 text-sm-h4">Villa kom upp</h2>
      </template>

    </div>
  </v-container>
</template>

<script>
export default {
  props: ['error']
}
</script>
