<template>
  <v-container class="">
      <div class="text-center">
          <v-row>
            <v-col cols="6" md="4" class="px-2"
            v-for="product in products" :key="product">
            <div class="img-top">
              <v-card  flat>
                <v-img
                    alt="Vuetify Logo"
                
                    :src="product.image" />
                </v-card>
            </div>
                
                <div class="mt-1 img-text py-3">
                    {{product.head}}
                </div>
                
            </v-col>
            </v-row>
      </div>
  
   
  </v-container>
</template>
<script>
import sub1 from "@/assets/images/sub1.png";
import sub2 from "@/assets/images/sub2.png";
import sub3 from "@/assets/images/sub3.png";
  export default {
    name: 'HelloWorld',
     data: () => {
    return {
        products: [
            {
                image: sub1,
                head: "Men Henley Neck",
            },
             {
                image: sub2,
                head: "Men Henley Neck",
            },
             {
                image: sub3,
                head: "Men Henley Neck",
            },
             {
                image: sub1,
                head: "Men Henley Neck",
            },
             {
                image: sub2,
                head: "Men Henley Neck",
            },
             {
                image: sub3,
                head: "Men Henley Neck",
            },
        ]
    }
  }
}
</script>
<style>
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
.img-top {
  position: relative !important;
  height: 158px;
}

.img-text{
  font-size: 14px !important;
  top: 70% !important;
  left: 50%;
  background: rgba(78, 75, 75, 0.25) !important;
  color: white;
  width: 100%;
  backdrop-filter: blur(10px) !important;
  
}
.multiPro{
  height: 340px !important;
  width: 100%;
}
@media only screen and (min-width: 960px) {
  .multiPro{
  height: 452px;
  width: 100%;
}
.offer-img{
    width: 100%;
    height: 276px;
}
.img-top {
  position: relative !important;
  height: 432px;
}

.img-text{
  font-size: 14px !important;
  top: 70% !important;
  left: 50%;
  background: rgba(78, 75, 75, 0.25) !important;
  color: white;
  width: 100%;
  backdrop-filter: blur(10px) !important;
  
}
}

</style>

