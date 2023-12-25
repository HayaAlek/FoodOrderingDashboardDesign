<template>
    <v-col cols="12" sm="8">
         <!------------------------------- Search ------------------------------->
            <v-text-field
              density="compact"
              placeholder="Search restaurant, Food, Cuisine or a Dish"
              append-inner-icon="mdi-magnify"
              variant="outlined"
              rounded
              class="text-grey mx-8"
            ></v-text-field>
             <!------------------------------- Categories------------------------------->
            <v-toolbar class="pr-1 mt-n7" color="transparent">
              <v-toolbar-title class="text-white">Categories</v-toolbar-title>
              <v-spacer></v-spacer>
              <span class="text-caption text-white">View all</span>
              <v-btn
                density="compact"
                icon="mdi mdi-chevron-right-box"
                color="grey"
              >
              </v-btn>
            </v-toolbar>
            <h6 class="text-white ml-4 mt-n4">
              <span class="text-red">10+ new</span> Categories added this week
            </h6>
            <!------------------------------- Popular Dishes------------------------------->

            <div class="d-flex justify-space-evenly mt-4" color="transparent">
              <v-avatar
                color="#605850"
                size="70"
                v-for="(food, index) in foods"
                :key="index"
              >
                <v-img :src="food.image"></v-img>
              </v-avatar>
            </div>
            <v-toolbar color="transparent" class="pr-1 mt-n2">
              <v-toolbar-title class="text-white"
                >Popular Dishes</v-toolbar-title
              >
              <v-spacer></v-spacer>
              <span class="text-caption text-white">View More</span>
              <v-btn
                density="compact"
                icon="mdi mdi-chevron-right-box"
                color="grey"
              >
              </v-btn>
            </v-toolbar>
            <h6 class="text-white ml-4 mt-n4">
              <span class="text-red">20+ new</span> Dishes added this week
            </h6>

            <div class="d-flex justify-space-evenly mt-4" color="transparent">
              <v-card color="transparent" v-for="(dishe, i) in dishes" :key="i">
                <v-img height="70" :src="dishe.image" class="imag"></v-img>
                <v-card class="mt-n10" width="160" color="#303030">
                  <v-card-item class="text-center">
                    <v-card-title class="mt-10">{{ dishe.name }}</v-card-title>
                    <v-card-subtitle>
                      <span class="me-1">Starting From</span>
                    </v-card-subtitle>
                    <v-card-title>{{ dishe.money }}</v-card-title>
                  </v-card-item>

                  <v-card-text>
                    <v-row align="center" class="mx-0">
                      <v-icon color="yellow" icon="mdi mdi-star" size="small">
                      </v-icon>
                      <div class="text-grey ms-4">
                        <h6>{{ dishe.star }}</h6>
                      </div>
                      <v-spacer></v-spacer>
                      <div class="text-grey ms-4">
                        1360
                        <h5>Total Sale</h5>
                      </div>
                    </v-row>
                  </v-card-text>
                </v-card>
              </v-card>
            </div>
            <!------------------------------- Order Reports------------------------------->
            <v-toolbar color="transparent" class="pr-1 mt-n2">
              <v-toolbar-title class="text-white"
                >Order Reports</v-toolbar-title
              >
              <v-spacer></v-spacer>
              <span class="text-caption text-white">View all</span>
              <v-btn
                density="compact"
                icon="mdi mdi-chevron-right-box"
                color="grey"
              ></v-btn>
            </v-toolbar>
            <h6 class="text-white ml-4 mt-n4">
              <span class="text-red"> Wow 1000+ new</span> Order got this week
            </h6>
            <v-card class="rounded-xl ma-2 pa-1" color="#424343">
              <v-row>
                <v-col cols="12" sm="1"> </v-col>
                <v-col cols="12" sm="2" class="text-center">
                  <span class="text-caption"> Customer</span>
                </v-col>
                <v-col cols="12" sm="2" class="text-center">
                  <span class="text-caption"> Order Number</span>
                </v-col>
                <v-col cols="12" sm="2" class="text-center">
                  <span class="text-caption"> Address</span>
                </v-col>
                <v-col cols="12" sm="2" class="text-center">
                  <span class="text-caption"> Amount</span>
                </v-col>
                <v-col cols="12" sm="2" class="text-center">
                  <span class="text-caption"> Status</span>
                </v-col>
                <v-col cols="12" sm="1" class="text-center">
                  <span class="text-caption"> </span>
                </v-col>
              </v-row>
            </v-card>
            <!------------------First Person--------------------- -->
            <v-row>
              <v-col cols="12" sm="3">
                <v-avatar>
                  <v-img src="20.jpg"></v-img>
                </v-avatar>
                <span class="text-caption text-white ml-1"> Sara John </span>
              </v-col>
              <v-col class="text-center mt-2" cols="12" sm="2">
                <span class="text-caption text-white">0123455664 </span>
              </v-col>
              <v-col class="mt-2 text-center" cols="12" sm="2">
                <span class="text-caption text-white">New York</span>
              </v-col>
              <v-col class="mt-2 text-center" cols="12" sm="2">
                <span class="text-caption text-white">$230.33 </span>
              </v-col>
              <v-col class="text-center" cols="12" sm="2">
                <v-ship variant="flat" color="green">Completed</v-ship>
              </v-col>
              <v-col class="text-center" cols="12" sm="1"> </v-col>
            </v-row>
            <!------------------Second Person-------------------- -->
            <v-row class="mt-n5">
              <v-col cols="12" sm="3">
                <v-avatar>
                  <v-img src="30.jpg"></v-img>
                </v-avatar>
                <span class="text-caption text-white ml-1"> Ali Ahmad </span>
              </v-col>
              <v-col class="text-center mt-2" cols="12" sm="2">
                <span class="text-caption text-white">0123479277 </span>
              </v-col>
              <v-col class="mt-2 text-center" cols="12" sm="2">
                <span class="text-caption text-white">Germany </span>
              </v-col>
              <v-col class="mt-2 text-center" cols="12" sm="2">
                <span class="text-caption text-white">$130.23 </span>
              </v-col>
              <v-col class="text-center" cols="12" sm="2">
                <v-ship variant="flat" color="Orange">Pending</v-ship>
              </v-col>
              <v-col class="text-center" cols="12" sm="1"> </v-col>
            </v-row>
          </v-col>
</template>
<script setup>
const foods = [
  { image: "2.png" },
  { image: "3.png" },
  { image: "4.png" },
  { image: "5.png" },
  { image: "6.png" },
  { image: "7.png" },
  { image: "8.png" },
];
const dishes = [
  { image: "11.png", name: "Hamburger", money: "$10.00", star: "4.5" },
  { image: "22.png", name: "Pizza", money: "$25.00", star: "4.1" },
  { image: "33.png", name: "Sushi", money: "$15.00", star: "4.3" },
  { image: "44.png", name: "Gratin", money: "$23.00", star: "4.9" },
];

</script>
<style>
.mRight {
  margin-right: 100px;
}
.v-list {
  background: transparent !important;
}
.mLeft {
  margin-left: 90px;
}
.imag {
  z-index: 9999 !important;
}
</style>
