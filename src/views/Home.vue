<template>
  <div class="home">
    <v-row justify="center" align="center">
      <v-col lg="2">
      <v-navigation-drawer width="350px" style="background:rgb(7,15,19);" absolute permanent>
        <template v-slot:prepend  >
          <img src="logo.png" height="120px" width="290px" class="pt-7 pl-16">
            <div class="text-center mt-5" >
              <v-icon x-small class="grey--text">control_camera</v-icon>
              <v-icon x-small class="grey--text ml-3">control_camera</v-icon>
              <v-icon x-small class="grey--text ml-3">control_camera</v-icon>
<br>
              <p text class="grey--text body-1 mt-4 mb-3">FR / EN</p>
<br>
              <v-list dense class="text-center">
                <v-list-item two-line v-for="item in items" :key="item.title">
                  <v-list-item-content>
                    <v-list-item-title class="body-1 grey--text my-2">
                      {{ item.title }}
                    </v-list-item-title>
                    <v-list-item-subtitle>
                      <v-icon class="grey--text">maximize</v-icon>
                    </v-list-item-subtitle>
                  </v-list-item-content>
                </v-list-item>
              </v-list>
<br>
              <v-icon x-small class="grey--text">control_camera</v-icon>
              <v-icon x-small class="grey--text ml-3">control_camera</v-icon>
              <v-icon x-small class="grey--text ml-3">control_camera</v-icon>
<br><br>
              <p class="grey--text mt-5 " style="font-size:0.6rem;">FOLLOW US</p>
              <img src="footer.png" height="50px" class="mb-3">
              <p class="grey--text mx-16" style="font-size:0.6rem;">© 2021, SPECTRE - ALL RIGHTS RESERVED WORDPRESS BY COLORZ </p>
            </div>
        </template>
      </v-navigation-drawer>
      </v-col>
      <v-col lg="10" class="justify-center">
        <v-img src="home-bg.jpg" height="820px"  >
          <div id="content" class="text-center"  >
            <h1 class="white--text">PREMIUM MUSIC AND <br> SOUND DESIGN</h1>
            <p class="white--text mt-5 ">THE ART OF TRANSLATING YOUR IDENTITY INTO MUSIC</p>
             <v-icon x-small class="white--text">control_camera</v-icon>
              <v-icon x-small class="white--text ml-5">control_camera</v-icon>
              <v-icon x-small class="white--text ml-5">control_camera</v-icon>
            <p class="body-1 white--text mt-10">We are expert in Retail Music Marketing. Our artistic and technical turnkey solutions combined with our extensive knowledge of retail marketing make our company your best music partner to support all your in and out store trading-up strategies.</p>
            <v-btn text class="px-10 py-5 white--text mt-10" style="border: 2px solid white;">LEARN MORE ABOUT US</v-btn>
          </div>
        </v-img>
      </v-col>
    </v-row>
  </div>
</template>

<script>
// @ is an alias to /src


export default {
  name: 'Home',
  data () {
      return {
        items: [
          { title: 'About', },
          { title: 'Activities', },
          { title: 'News',  },
          { title: 'Contact',  },
        ],
      }
    },
}
</script>

<style >
#content{
  margin-top: 220px;
}
#content h1{
  font-size: 2rem;
  letter-spacing: 10px;
}
#content p{
  font-size: 1rem;
  margin-right: 400px;
  margin-left: 400px;
}
</style>