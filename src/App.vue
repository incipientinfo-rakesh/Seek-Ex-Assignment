<template>
  <v-app>
    <v-app-bar
      app
      color="#FFFFFF"
      dark
    >
      <div class="d-flex align-center ml-md-16">
        <v-img
          alt="Vuetify Logo"
          src="@/assets/images/Vector.svg"
          width="18"/>
      </div>
      <v-spacer></v-spacer>

      <div class="text-black font-16">
        Logo Here
      </div>
     
      <v-spacer></v-spacer>

      <!-- <v-btn
        href="https://github.com/vuetifyjs/vuetify/releases/latest"
        target="_blank"
        text
      >
        <span class="mr-2">Latest Release</span>
        <v-icon>mdi-open-in-new</v-icon>
      </v-btn> -->
      <div class="d-flex mr-md-16">
        <div class="mx-4">
          <v-img
          class="header-icon justify-space-between"
          alt="Vuetify Logo"
          src="@/assets/images/search.svg"
          />
        </div>
      
        <div class="mx-4">
          <v-img
          class="header-icon"
          alt="Vuetify Logo"
          src="@/assets/images/like.svg"
          />
        </div>
          
        <div class="mx-4">
          <v-img
          class="header-icon"
          src="@/assets/images/shop.svg"
          />
        </div>
          
        <div class="mx-4">
            <v-img
          class="header-icon-acc"
          src="@/assets/images/account.svg"
          />
        </div>
          </div>
    </v-app-bar>

    <v-main>
      <router-view/>
    </v-main>
  </v-app>
</template>

<script>

export default {
  name: 'App',

  data: () => ({
    //
  }),
};
</script>
<style>
.header-icon{
  max-width: 18px !important;
 
}
.header-icon-acc{
  max-width: 15px !important;
}
.text-black{
  color: #1C1C1C;
}
.font-16{
  font-size: 16px;
  font-family: Playfair Display;
  font-weight: 600;
}

</style>

