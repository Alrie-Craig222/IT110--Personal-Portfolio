<!-- <template>
  <div class="about">
    <h1>This is an about page</h1>
  </div>
</template> -->


<template>
  <a name="about"></a>
  <v-container>
    <section class="mt-15">
      <h4 class="text-h4 text-center mb-5">About Me</h4>
      <v-row class="align-center justify-center">
        <v-col>
          <v-card class="text-center pa-6 rounded-lg" color="black" elevation="6">
            <v-card-subtitle class="text-h5 text-white">ABOUT ME</v-card-subtitle>
            <h2 class="display-1 font-weight-regular mt-5 text-white">
              I’m a passionate Full Stack Web Developer with a love for crafting clean, 
              functional, and intuitive web experiences. Every line of code is a step toward 
              solving a puzzle, and I’m always on the lookout for the next challenge to unravel. 
              From building sleek frontends to designing robust backends, I bring ideas to life, 
              one project at a time. Curious by nature, I prefer letting my work speak for itself—there’s 
              always more to discover beneath the surface.
            </h2>
            <div class="d-flex justify-center text-white">
              <v-btn href="#" large elevation="5" color="#c00472" class="text-white mt-5 px-10 py-5 d-flex justify-space-around align-center flex-column flex-md-row">
                Learn More
                <v-icon>mdi-gesture-tap</v-icon>
              </v-btn>
            </div>
          </v-card>
        </v-col>
        </v-row>
        <br><br>
        <v-row class="align-center justify-center">
        <v-col>
          <v-card class="pa-6 rounded-lg" color="black" elevation="6">
            <v-card-subtitle class="text-white text-center text-h5">LANGUAGES & TECHNOLOGIES</v-card-subtitle><br>
            <div class="py-1 text-white" v-for="(item, index) in items" :key="index"><br>
              <label>{{ item.title }}</label>
              <v-progress-linear :color="item.color" height="5" buffer-value="0" :model-value="item.value" stream></v-progress-linear>
            </div>
          </v-card>
        </v-col>
      </v-row>
    </section>
  </v-container>
</template>

<script setup>
const items = [
  { title: 'Python', value: 75, color: '#c00472' },
  { title: 'HTML', value: 80, color: '#c00472' },
  { title: 'CSS', value: 75, color: '#c00472' },
  { title: 'Javascript', value: 75, color: '#c00472' },
  { title: 'VueJS', value: 50, color: '#c00472' },
  { title: 'Vuetify', value: 50, color: '#c00472' },
  { title: 'C', value: 65, color: '#c00472' },
  { title: 'Java', value: 50, color: '#c00472' },
];

</script>

