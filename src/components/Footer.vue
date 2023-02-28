<template>
<div class="suport">
  <v-container class="">
      <div class="">
          <v-row class="my-10 d-flex">
            <v-col  class="mr-md-2 px-0">
               <div class="mx-4">
                   Lorem ipsum dolor sit amet consectetur adipisicing elit. Voluptates, amet. Ad hic vero modi consectetur corrupti reprehenderit vel, itaque cupiditate doloremque fuga iste, commodi eius repellat recusandae dolor. Accusamus, maiores?
               </div>
            </v-col>
            <v-col  class="ml-md-2 px-0 pl-md-10 mx-4">
                    <div class="font-18e">ONLINE SHOPPING</div>
                    <div class="mt-2">Men’s T-Shirts</div>
                    <div class="mt-2">Women’s Wear</div>
                    <div class="mt-2">Winter Collections</div>
                    <div class="mt-2">Hooded T-Shirts</div>
                    <div class="mt-2">Streetwear Collections</div>
            </v-col>
            <v-col  class="ml-md-2 px-0 mx-4">
               <div class="font-18e">CUSTOMER POLICIES</div>
               <div class="mt-2">About Us</div>
                <div class="mt-2">Terms & Conditions</div>
                <div class="mt-2">Shipping & Returns Policy</div>
                <div class="mt-2">Cancellation & Refund Policy</div>
                <div class="mt-2">Contact Us</div>
            </v-col>
            <v-col  class="ml-md-2 px-0 mx-4">
                <div class="font-18e">STORE INFORMATION</div>
                <div class="mt-2 d-flex">
                    <span>
                          <v-img alt="Vuetify Logo" class="icon mr-3 mt-1" width="15px" src="@/assets/images/location.svg"/>
                    </span>

                    Lorem Ipsum is simply dummy text of the
                    printing and typesetting industry. </div>
                <div class="mt-2 d-flex">
                    <span>
                        <v-img alt="Vuetify Logo" class="icon mr-3 mt-1" width="15px" src="@/assets/images/phone.svg" />
                    </span>
                    Call Us: 1234567890</div>
                <div class="mt-2 d-flex">
                    <span>
                        <v-img alt="Vuetify Logo" class="icon mr-3 mt-1" width="15px" src="@/assets/images/email.svg" />
                    </span>
                    Email Us: info@yourmail.com</div>
            </v-col>
            </v-row>
      </div>
  </v-container>
   <v-footer dark padless >
    <v-card class="flex" flat tile color="#20050A">
      <v-card-text class="py-2 white--text text-center">
        <strong>©2022-23 Powered By dummy team</strong>
      </v-card-text>
    </v-card>
  </v-footer>
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
.font-18e{
    font-size: 18px;
    font-family: Playfair Display;
    font-weight: 600;
    color: #770015;
}
/* .offer-img{
    width: 375px;
    height: 176px;
} */
@media only screen and (min-width: 960px) {
/* .offer-img{
    width: 100%;
    height: 100%;
} */
}
</style>

