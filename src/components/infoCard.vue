<template>
    <v-col cols="12" sm="4">
            <v-card color="#4e4e4e" height="655" class="rounded-xl">
              <v-card
                class="mx-2 mt-4 rounded-lg"
                max-width="344"
                color="#6d6d6d"
              >
                <v-card-item title="Delivery Address">
                  <template v-slot:subtitle>
                    <v-icon
                      icon="mdi mdi-map-marker"
                      size="18"
                      class="me-1 pb-1"
                    ></v-icon>

                    Po.1478, Street No. 52 West New York
                  </template>
                </v-card-item>

                <v-card-text class="mt-n3">
                  <v-icon
                    size="16"
                    icon="mdi mdi-clock-outline"
                    class="mr-2"
                  ></v-icon
                  >20 min</v-card-text
                >
              </v-card>
              <v-toolbar color="transparent" class="pr-1 mt-n2">
                <v-btn icon class="hidden-xs-only">
                  <v-icon>mdi mdi-cart</v-icon>
                </v-btn>
                <v-toolbar-title>Cart</v-toolbar-title>
                <v-spacer></v-spacer>
                <span class="text-caption">Order ID: #1099</span>
              </v-toolbar>
              <v-card class="rounded-xl ma-2 pa-1 mt-n2" variant="outlined">
                <v-chip variant="flat" color="red">Delivery</v-chip>
                <v-chip variant="text" class="ml-5">Dine in</v-chip>
                <v-chip variant="text" color="red">|</v-chip>
                <v-chip variant="text">Takeaway</v-chip>
              </v-card>
              <v-card
                class="ma-2 mt-n2"
                title="Pepperoni Pizza"
                subtitle="Thin Crust"
                color="transparent"
                flat
              >
                <template v-slot:prepend>
                  <v-avatar>
                    <v-img src="1.webp"></v-img>
                  </v-avatar>
                </template>
                <template v-slot:append>
                  <v-btn
                    density="compact"
                    icon="mdi mdi-circle-edit-outline"
                    x-small
                  ></v-btn>
                </template>
                <v-card-text class="ml-14 mt-n2">
                  <v-icon class="mr-2" x-small
                    >mdi mdi-plus-circle-outline</v-icon
                  >2
                  <v-icon class="ml-1" x-small
                    >mdi mdi-minus-circle-outline</v-icon
                  >
                </v-card-text>
              </v-card>

              <v-divider class="mt-n2" inset></v-divider>
              <v-card
                class="ma-2 mt-2"
                title="Cheese Burger"
                subtitle="Whole wheat bun"
                color="transparent"
                flat
              >
                <template v-slot:prepend>
                  <v-avatar>
                    <v-img src="2.png"></v-img>
                  </v-avatar>
                </template>
                <template v-slot:append>
                  <v-btn
                    density="compact"
                    icon="mdi mdi-circle-edit-outline"
                    x-small
                  ></v-btn>
                </template>
                <v-card-text class="ml-14 mt-n2">
                  <v-icon class="mr-2" x-small
                    >mdi mdi-plus-circle-outline</v-icon
                  >14
                  <v-icon class="ml-1" x-small
                    >mdi mdi-minus-circle-outline</v-icon
                  >
                </v-card-text>
              </v-card>

              <v-card class="rounded-xl ma-2 pa-1 mt-n2" elevation="16">
                <v-chip variant="text" class="mRight">Promotion Code</v-chip>
                <v-chip variant="flat" color="black">TRYNEW</v-chip>
              </v-card>

              <v-card color="transparent" class="ma-2" flat>
                <v-list class="text-white" density="comfortable">
                  <v-list-item title="Sub total">
                    <template v-slot:append>
                      <v-btn variant="text">$155.20</v-btn>
                    </template>
                  </v-list-item>
                  <v-list-item title="Delivery Charge">
                    <template v-slot:append>
                      <v-btn variant="text">$10</v-btn>
                    </template>
                  </v-list-item>
                  <v-divider inset></v-divider>
                  <v-list-item title="Total">
                    <template v-slot:append>
                      <v-btn variant="text">$170.99</v-btn>
                    </template>
                  </v-list-item>
                </v-list>
              </v-card>

              <v-chip variant="flat" color="black" class="px-10 mLeft"
                >Confirm Order</v-chip
              >
            </v-card>
          </v-col>
</template>
<script></script>