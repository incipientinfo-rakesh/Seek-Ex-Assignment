<template>
  <v-container class="mt-16">
      <div>
          <v-row>
            <v-col class="mr-md-2 px-0">
                <v-img
                    alt="Vuetify Logo"
                    class="offer-img"
                    src="@/assets/images/brandoff.png"/>
            </v-col>
            <v-col class="ml-md-2 px-0">
                <v-img
                    alt="Vuetify Logo"
                    class="offer-img"
                    src="@/assets/images/brandoff2.png"/>
            </v-col>
            </v-row>
      </div>
  </v-container>
</template>
<script>
  export default {
    name: 'HelloWorld',
    data: () => ({
    }),
  }
</script>
<style>
.offer-img{
    width: 100%;
    height: 100%;
}
@media only screen and (min-width: 960px) {
.offer-img{
    width: 100%;
    height: 100%;
}
}
</style>

