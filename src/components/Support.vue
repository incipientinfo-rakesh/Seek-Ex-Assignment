<template>
<div class="suport">
  <v-container class="mt-16">
      <div class="justify-center" align="center">
          <v-row class="my-10">
            <v-col class="mr-md-2 px-0">
                <v-img
                    alt="Vuetify Logo"
                    class="icon"
                    src="@/assets/images/icon1.svg"/>
                    <div class="mt-10">7 Days Return</div>
                    
            </v-col>
            <div class="vl"></div>
            <v-col class="ml-md-2 px-0">
                <v-img
                    alt="Vuetify Logo"
                    class="icon"
                    src="@/assets/images/icon2.svg"/>
                    <div class="mt-6">Quality Products</div>
            </v-col>
            <div class="vl"></div>
            <v-col class="ml-md-2 px-0">
                <v-img
                    alt="Vuetify Logo"
                    class="icon"
                    src="@/assets/images/icon3.svg"/>
                    <div class="mt-10">Safe Payment</div>
            </v-col>
            <div class="vl"></div>
            <v-col class="ml-md-2 px-0">
                <v-img
                    alt="Vuetify Logo"
                    class="icon"
                    src="@/assets/images/icon4.svg"/>
                    <div class="mt-10">24x7 Helpline</div>
            </v-col>
            </v-row>
      </div>
  </v-container>
  </div>
</template>
<script>
  export default {
    name: 'HelloWorld',
    data: () => ({
    }),
  }
</script>
<style>
.support{
    background-color: #F5F4F2 !important;
}
.vl {
  border-left: 1px solid #FFC7D1;
  height: 180px;
}
.icon{
    width: 40px;
}
/* .offer-img{
    width: 375px;
    height: 176px;
} */
@media only screen and (min-width: 960px) {
.icon{
    width: 80px;
}
/* .offer-img{
    width: 100%;
    height: 100%;
} */
}
</style>

