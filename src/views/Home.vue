<template>
  <v-app
    id="inspire"
    :style="{ background: $vuetify.theme.themes.light.colors.primary }"
  >
    <!-----------------------Side Bar----------------------------->

    <SideBar />
    <v-main>
      <v-container>
        <v-row>
          <!-----------------------Main Content----------------------------->
          <mainContent />
          <!-----------------------Information Card----------------------------->
          <infoCard />
        </v-row>
      </v-container>
    </v-main>
  </v-app>
</template>

<script setup>
import SideBar from "@/components/SideBar.vue";
import infoCard from "@/components/infoCard.vue";
import mainContent from "@/components/mainContent.vue";
</script>

