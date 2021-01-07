<template>
  <div class="home">
      <v-navigation-drawer width="370px" style="background:rgb(7,15,19);" absolute permanent>
        <template v-slot:prepend  >
          <img src="logo.png" height="155px" width="320px" class="pt-10 pl-10">
            <div class="text-center grey--text mt-5" >
              <v-icon x-small class="grey--text">control_camera</v-icon>
              <v-icon x-small class="grey--text">control_camera</v-icon>
              <v-icon x-small class="grey--text">control_camera</v-icon>
<br>
              <p text class="grey--text mb-3">FR / EN</p>
<br>
              <v-list dense class="text-center">
                <v-list-item two-line v-for="item in items" :key="item.title">
                  <v-list-item-content>
                    <v-list-item-title class="title grey--text my-2">
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
              <v-icon x-small class="grey--text">control_camera</v-icon>
              <v-icon x-small class="grey--text">control_camera</v-icon>
<br><br>
              <p class="grey--text mt-5 caption">FOLLOW US</p>
              <img src="footer.png" height="50px" class="mb-3">
              <p class="grey--text caption mx-7">© 2021, <a href="https://github.com/Abir-Bouhriz"  >BOUHRIZ ABIR</a> </p>
            </div>
        </template>
      </v-navigation-drawer>
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
.mt-n2 a{
  text-decoration: none;
  color: grey !important;
}
.mt-n2  a:hover{
  color: white !important;
}
</style>