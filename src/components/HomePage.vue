<template>
  <v-container>
    <v-row class="d-flex justify-center">
      <v-col cols="8" sm="5" md="4" class="body d-flex flex-column">
        <v-col class="d-flex justify-center pa-0 mt-15"
          ><img class="image" src="/src/assets/pic.png" alt=""
        /></v-col>

        <v-col class="text name pa-0 text-center mt-3 mb-1">
          Abhishek Negi
          <span class="text-grey-darken-1 ml-1">29</span>
        </v-col>
        <v-col class="text place pa-0 text-center">Bangalore</v-col>

        <div class="line d-flex justify-center mt-4 mb-4"></div>
        <v-divider></v-divider>
        <v-col class="stats d-flex pa-0 mb-2">
          <v-col cols="4" class="d-flex flex-column pa-0 text-center">
            <v-col class="text1 pa-0">80K</v-col>
            <v-col class="text2 pa-0">Followers</v-col>
          </v-col>
          <v-col cols="4" class="d-flex flex-column pa-0 text-center">
            <v-col class="text1 pa-0">803K</v-col>
            <v-col class="text2 pa-0">Likes</v-col>
          </v-col>
          <v-col cols="4" class="d-flex flex-column pa-0 text-center">
            <v-col class="text1 pa-0">1.4K</v-col>
            <v-col class="text2 pa-0">Photos</v-col>
          </v-col>
        </v-col>
      </v-col>
    </v-row>
  </v-container>
</template>

<script setup>
</script>

<style scoped>
@font-face {
  font-family: f1;
  src: url(/src/assets/KumbhSans-Bold.ttf);
}
@font-face {
  font-family: f2;
  src: url(/src/assets/KumbhSans-Light.ttf);
}
.body {
  background-color: #ffffff;
  border-radius: 15px;
  background-image: url("/src/assets/bg-pattern-card.svg"); /* Set the background image */
  background-size: 100% 35%; /* Make the image take 40% of the background from the top */
  background-repeat: no-repeat; /* No repeating of the image */
  background-position: top; /* Place the background image at the top */
}
.image {
  width: 35%;
  border-radius: 50%; /* Circular border */
  border: 4px solid white; /* White border around the image */
}
.text {
  color: hsl(229, 23%, 23%);
}
.text1 {
  color: hsl(229, 23%, 23%);
  font-family: f1;
  font-size: 18px;
}
.text2 {
  color: hsl(229, 23%, 23%);
  font-family: f2;
  font-size: 8px;
  letter-spacing: 1px;
}
.place {
  font-size: 13px;
}
.line {
  height: 1px;
  width: 109.5%;
  background-color: hsla(0, 0%, 59%, 20%);
  margin: 0; /* Remove default margin */
  padding: 0; /* Remove default padding */
  box-sizing: border-box; /* Ensure padding doesn't affect the width */
  position: relative; /* Relative positioning for fine adjustment */
  left: -12px; /* Move the line 10px to the left */
}
</style>