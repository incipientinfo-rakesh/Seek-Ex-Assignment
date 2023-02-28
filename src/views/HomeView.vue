<template>
<div>
  <div class="main-img">
    <v-img
        alt="Vuetify Logo"
        class="banner-img"
        src="@/assets/images/banner.png"/>
  </div>
  <div class="container mt-16" align="center">
    <v-row>
      <v-col v-for="item in items" :key="item" cols="6" md="2">
        <v-img
        alt="Vuetify Logo"
        class="model-img"
        :class="item.bgcolor"
        :src="item.image"/>
        <div class="text-center font-16 mt-3">{{item.text}}</div>
      </v-col>
    </v-row> 
  </div>
  <OfferSection />
  <div>
    <div class="d-flex container">
      <v-divider class="mt-14 mr-5"></v-divider>
      <div class="font-36 text-center my-6">Trending T-Shirts</div>
      <v-divider class="mt-14 ml-5"></v-divider>
    </div>
     <ProductView />
     <ProductView class=""/>
      <div class="py-7 text-center">
      <v-btn class="vue-btn px-7 px-md-10 rounded-md"
        >View All</v-btn
      >
    </div>
  </div>
  <div class="mt-4">
    <div class="d-flex container">
      <v-divider class="mt-14 mr-5"></v-divider>
      <div class="font-36 text-center mt-6">Featured Products</div>
      <v-divider class="mt-14 ml-5"></v-divider>
    </div>
     <ProductView class=""/>
      <div class="py-7 text-center">
      <v-btn class="vue-btn px-7 px-md-10 rounded-md"
        >View All</v-btn
      >
    </div>
  </div>
  <div class="main-img">
    <v-img
        alt="Vuetify Logo"
        class="banner-img"
        src="@/assets/images/banner2.png"/>
  </div>
   <div class="mt-4">
     <div class="d-flex container">
      <v-divider class="mt-14 mr-5"></v-divider>
      <div class="font-36 text-center mt-6">New Products</div>
      <v-divider class="mt-14 ml-5"></v-divider>
    </div>
     <ProductView class=""/>
      <div class="py-7 text-center">
      <v-btn class="vue-btn px-7 px-md-10 rounded-md"
        >View All</v-btn
      >
    </div>
  </div>
  <div class="mt-4">
    <div class="d-flex container">
      <v-divider class="mt-14 mr-5"></v-divider>
      <div class="font-36 text-center mt-6">Best Selling Products</div>
      <v-divider class="mt-14 ml-5"></v-divider>
    </div>
     <ProductView class="mt-4"/>
      <div class="py-7 text-center">
      <v-btn class="vue-btn px-7 px-md-10 rounded-md"
        >View All</v-btn
      >
    </div>
  </div>
  <MultiPro />
  <div class="main-img mt-10">
    <v-img
        alt="Vuetify Logo"
        class="banner-img"
        src="@/assets/images/banner3.png"/>
  </div>
 <BrandOffer />
 <Support class="support"/>
 <div class="main-img mt-10">
   <v-container>
     <v-img
        alt="Vuetify Logo"
        class="banner-5"
        src="@/assets/images/banner5.png"/>
   </v-container>
  </div>
  <v-divider></v-divider>
  <Footer />

</div>
  
</template>

<script>
 
  import OfferSection from '../components/OfferSection'
  import ProductView from '../components/ProductView'
  import MultiPro from '../components/MultiPro';
  import BrandOffer from '../components/BrandOffer';
  import Support from '../components/Support';
  import Footer from '../components/Footer';
  import model1 from "@/assets/images/model1.png";
  import model2 from "@/assets/images/model2.png";
  import model3 from "@/assets/images/model3.png";
  import model4 from "@/assets/images/model4.png";
  import model5 from "@/assets/images/model5.png";
  import model6 from "@/assets/images/model6.png";

  export default {
    name: 'HomeView',

    components: {
      ProductView,
      OfferSection,
      MultiPro,
      BrandOffer,
      Support,
      Footer
    },
     data: () => {
    return {
    items: [
      {
        bgcolor: 'model1',
        image: model1,
        text: "Men's T-shirts"
      },
       {
        bgcolor: 'model2',
        image: model2,
        text: "Women's Wear"
      },
      {
        bgcolor: 'model3',
        image: model3,
        text: "Winter Collections"
      },
      {
        bgcolor: 'model4',
        image: model4,
        text: "Hooded T-Shirts"
      },
      {
        bgcolor: 'model5',
        image: model5,
        text: "Polo Neck T-Shirts"      },
      {
        bgcolor: 'model6',
        image: model6,
        text: "Full Sleeves T-Shirts"
      },
      
    ]
    }
    }
  }
</script>
<style>
.vue-btn{
  background-color: #770015 !important;
  color: #ffffff !important;
}
.banner-5{
  width: 100%;
  height: 100% !important;
}
.banner-img{
  width: 100%;
  height: 100% !important;
}
.model-img{
 position: relative;
  width: 120px;
  height: 120px;
  border-radius: 100px;
}
.model1{
  background: #F1DBE9;
}
.model2{
  background: #DDD3EB;
}
.model3{
  background:#D3EAEB;
}
.model4{
  background: #EFF1D9;
}
.model5{
  background: #F1DADB;
}
.model6{
  background: #D9F1DE;
}
@media only screen and (min-width: 960px) {
  .banner-5{
  width: 100%;
  height: 312px !important;
}
  .banner-img{
  width: 100%;
  height: 632px !important;
}
.model-img{
 position: relative;
  width: 170px;
  height: 170px;
  border-radius: 100px;
}
}


</style>

