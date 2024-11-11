<!-- <template>
  <v-app class="bg-grey-lighten-5">
    <SiteHeader />
    <v-main>
      <router-view />
    </v-main>
    <v-footer theme="dark" color="grey-lighten-2 mt-5">
      <v-container class="text-center w-100 justify-space-between d-flex flex-row">
        <v-row>
          <v-col>
            <div class="align-start">
              <div class="d-flex flex-row justify-start flex-column text-start">
                <p>You can find my projects in <strong><a href="#portfolio"
                      class="text-blue text-decoration-none">Portfolio</a></strong> part. </p>
                <p>For communication and your questions, you can send a form from the "<strong><a href="#contact"
                      class="text-blue text-decoration-none">contact me</a></strong>"
                  section.</p>
              </div>
            </div>
          </v-col>
        </v-row>
      </v-container>
    </v-footer>
    <div class="bg-grey-lighten-2 text-center d-flex flex-column">
      <v-divider></v-divider>
      <v-subheader>
        <strong>© <a href="https://github.com/onaranyusuf" class="text-red text-decoration-none">YUSUF ONARAN</a> —
          Theme by <a href="https://www.yusufonaran.me" target="_blank" class="text-red text-decoration-none">YUSUF
            ONARAN</a> </strong> — {{ new Date().getFullYear() }}
        <v-spacer></v-spacer>
      </v-subheader>
    </div>
  </v-app>
</template>

<script>
import SiteHeader from '@/components/header.vue';

export default {
  name: 'App',
  data: () => ({

  }),

  components: {
    SiteHeader,
  },

}
</script>
 -->


 <template>
  <nav>
    <v-btn><router-link to="/">Home</router-link></v-btn>
    <v-btn><router-link to="/about">About</router-link></v-btn>
    <v-btn><router-link to="/contacts">Contacts</router-link></v-btn>
    
  </nav>
  <router-view/>
</template>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #fff;
}

nav {
  display: flex;
  justify-content: center; /* Centers the buttons horizontally */
  align-items: center;
  gap: 20px; /* Adds space between the buttons */
  padding: 10px; /* Adds padding around the navbar */
  position: fixed; /* Keeps navbar at the top */
  top: 0; /* Positions the navbar at the very top */
  width: 100%; /* Makes navbar span the full width */
  background-color: rgba(51, 51, 51, 0.8); /* Background color for visibility */
  z-index: 1000; /* Ensures it stays on top of other elements */
}

nav a {
  font-weight: bold;
  text-decoration: none; /* Removes underline from links */
  color: inherit; /* Inherits the button's color */
}

nav a.router-link-exact-active {
  color: #fa48b0;
}
.v-btn {
  font-weight: bold;
  padding: 0 15px;
  background-color: #c00472;
}
/* To avoid content overlapping with the fixed navbar */
.router-view-container {
  padding-top: 80px; /* Adjust padding to match navbar height */
}
</style> 



