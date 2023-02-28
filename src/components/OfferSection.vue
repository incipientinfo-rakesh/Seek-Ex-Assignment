<template>
  <v-container class="mt-16">
      <div>
          <v-row>
            <v-col class="mr-md-2 px-0">
              <v-card flat>
                <v-img
                    alt="Vuetify Logo"
                    class="offer-img"
                    src="@/assets/images/offer1.png"/>
                  </v-card>
            </v-col>
            <v-col class="ml-md-2 px-0">
               <v-card flat>
                <v-img
                    alt="Vuetify Logo"
                    class="offer-img"
                    src="@/assets/images/offer2.png"/>
                 </v-card>
            </v-col>
            </v-row>
      </div>
    <v-row>
        <v-col cols="4" class="px-0 pr-2">
           <v-card flat>
            <v-img
             alt="Vuetify Logo"
             src="@/assets/images/offer3.png"/>
              </v-card>
        </v-col>
        <v-col cols="4" class="px-2">
          <v-card flat>
            <v-img
             alt="Vuetify Logo"
             src="@/assets/images/offer4.png"/>
             </v-card>
        </v-col>
        
        <v-col cols="4" class="px-0 pl-2">
          <v-card flat>
            <v-img
             alt="Vuetify Logo"
             src="@/assets/images/offer5.png"/>
             </v-card>
        </v-col>
    </v-row>
   
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
    width: 375px;
    height: 176px;
}
@media only screen and (min-width: 960px) {
.offer-img{
    width: 100%;
    height: 276px;
}
}
</style>

