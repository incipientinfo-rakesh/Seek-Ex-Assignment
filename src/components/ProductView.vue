<template>
  <v-container class="">
      <div class="text-center">
          <v-row>
            <v-col cols="6" md="3" class="px-2"
            v-for="product in products" :key="product.id">
            <v-card flat>
                <div class="hover-product">
                <v-img
                    alt="Vuetify Logo"
                    class="image"
                    :src="product.image"/>
                 <div class="middle d-flex">
                    <v-btn class="mx-2" fab dark small color="white">
                        <v-img alt="Vuetify Logo" class="" max-width="30px" src="@/assets/images/cart.svg"/>
                    </v-btn>
                    <v-btn class="mx-2" fab dark small color="white">
                        <v-img alt="Vuetify Logo" class="" max-width="25px" src="@/assets/images/heart.svg"/>
                    </v-btn>
                    <v-btn class="mx-2" fab dark small color="white">
                          <v-img alt="Vuetify Logo" class="" max-width="25px" src="@/assets/images/share.svg"/>
                    </v-btn>
                </div>
                <div class="mt-1">
                    {{product.head}}
                    <div>{{product.sub}}</div>
                </div>
                <div class="font-16">{{product.price}}</div>
                <div class="mt-2">
                    <v-btn variant="outlined" class="button px-2">S</v-btn>
                    <v-btn class="button mx-2" variant="outlined">M</v-btn>
                    <v-btn class="button" variant="outlined">L</v-btn>
                </div>
                </div>
                </v-card>
               
            </v-col>
            </v-row>
      </div>
  
   
  </v-container>
</template>
<script>
import product1 from "@/assets/images/product1.png";
import product2 from "@/assets/images/product2.png";
import product3 from "@/assets/images/product3.png";
import product4 from "@/assets/images/product4.png";
  export default {
    name: 'HelloWorld',
     data: () => {
    return {
        products: [
            {
                id: 0,
                image: product1,
                head: "Men Henley Neck",
                sub: "Full Sleeve Red Wine",
                price: 399,
            },
             {
                 id: 1,
                image: product2,
                head: "Men Henley Neck",
                sub: "Full Sleeve Red Wine",
                price: 399,
            },
             { 
                 id: 2,
                image: product3,
                head: "Men Henley Neck",
                sub: "Full Sleeve Red Wine",
                price: 399,
            },
             {
                 id: 3,
                image: product4,
                head: "Men Henley Neck",
                sub: "Full Sleeve Red Wine",
                price: 399,
            },
        ]
    }
  }
}
</script>
<style>


.image {
  opacity: 1;
  display: block;
  width: 100%;
  height: auto;
  transition: .5s ease;
  backface-visibility: hidden;
}

.middle {
  transition: .5s ease;
  opacity: 0;
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  -ms-transform: translate(-50%, -50%);
  text-align: center;
}

.container:hover .image:hover {
  opacity: 0.3;
}

.container:hover .middle:hover {
  opacity: 1;
}


/* ---------- */
.button{
    width: 50px;
}
.offer-img{
    width: 375px;
    height: 176px;
}
.font-36{
    font-size: 36px;
    font-weight: 600;
    font-family: Playfair Display;
}
.font-18{
    font-size: 18px;
    font-weight: 700;
    font-family: Playfair Display;
}
.v-btn:not(.v-btn--round).v-size--default{
    min-width: 35px !important;
}
@media only screen and (min-width: 960px) {
.offer-img{
    width: 100%;
    height: 276px;
}
}

</style>

