<template>
    <a name="resume"></a>
    <v-container fluid class="container-margin-top">
      <v-row>
        <!-- Left Section (Contact, References) -->
        <v-col cols="12" md="4" class="left-section pa-4 white--text">
          <v-card class="left_section" flat>
            <!-- Profile Picture -->
            <div class="profile-picture mb-4">
              <v-img
                :src="require('@/assets/pf.png')"
                alt="Profile Photo"
                height="200"
                width="200"
              ></v-img>
              </div>
  
  
            <!-- Contact Information -->
            <div class="left--section">
              <h3 class="mb-2 font-weight-bold">CONTACT</h3>
              <p>Buenavista, Butuan City, Philippines, 8601</p>
              <p>+639 3512345678</p>
              <p>alriecraig@gmail.com</p>
            </div>
            <br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br>
  
            <!-- References -->
            <div class="mt-6 left--section">
              <h3 class="mb-2 font-weight-bold">REFERENCES</h3>
              <p>Kakashi Hatake</p>
              <p>Software Engineering Manager | Konoha XYZ Technologies</p>
              <p>+1 416-888-3233</p>
              <p>kakashi.hatake@konohaxyztech.com</p>
              <br><br>
              <p>Itachi Uchiha</p>
              <p>Senior Backend Developer | Konoha XYZ Technologies</p>
              <p>+1-555-555-4444</p>
              <p>itachi.uchiha@konohaxyztech.com</p>
              <br><br>
            </div>
          </v-card>
        </v-col>
  
        <!-- Right Section (Main Resume) -->
        <v-col cols="12" md="8" class="right-section pa-4">
          <v-card class="right_section" flat>
            <!-- Name and Title -->
             <br>
            <h1 class="mb-2 font-weight-bold">ALMARIE MAESTRADO</h1>
            <h4 class="grey--text">Full Stack Web Developer</h4>
  
            <!-- Work Experience -->
            <div class="mt-6">
              <h3 class="font-weight-bold mb-2">WORK EXPERIENCE</h3>
              <v-timeline align-top dense>
                <v-timeline-item v-for="(item, i) in workExperience" :key="i">
                  <template #opposite>
                    <span>{{ item.year }}</span>
                  </template>
                  <template #default>
                   
                      <h4 class="mb-2 font-weight-bold">{{ item.company }}</h4>
                      <h6 class="grey--text">{{ item.position }}</h6>
                      <p>{{ item.description }}</p>
                    
                  </template>
                </v-timeline-item>
              </v-timeline>
            </div>
  
            <!-- Education -->
            <div class="mt-6">
              <h3 class="font-weight-bold mb-2">EDUCATION</h3>
              <v-timeline align-top dense>
                <v-timeline-item v-for="(item, i) in education" :key="i">
                  <template #opposite>
                    <span>{{ item.year }}</span>
                  </template>
                  <template #default>
                    
                      <h4 class="mb-2 font-weight-bold">{{ item.institution }}</h4>
                      <h6 class="grey--text">{{ item.degree }}</h6>
                    
                  </template>
                </v-timeline-item>
              </v-timeline>
            </div>
  
            <!-- Skills & Experience -->
            <div class="mt-6">
              <h3 class="font-weight-bold mb-2">SKILLS & EXPERIENCE</h3>
              <v-row>
                <v-col v-for="(skill, i) in skills" :key="i" cols="6" md="4">
                  <v-chip class="ma-1">{{ skill }}</v-chip>
                </v-col>
              </v-row>
            </div>
          </v-card>
        </v-col>
      </v-row>
    </v-container>
  </template>
  
  <script>
  export default {
    data() {
      return {
        workExperience: [
          {
            year: "Jan 2023 - Present",
            company: "ABC Technologies",
            position: "Full Stack Web Developer",
            description:
              "Developed and maintained an e-commerce platform using Vue.js and Node.js, creating RESTful APIs and integrating Stripe for payment processing. Enhanced database performance with PostgreSQL and migrated legacy systems to AWS, reducing costs. Automated deployment with Jenkins, improving release efficiency by 50%.",
          },
          {
            year: "May 2020 – Dec 2022",
            company: "XYZ Digital Solutions",
            position: "Full Stack Developer ",
            description:
              "Led the development of a SaaS application using React.js and Django, implemented secure user authentication with OAuth 2.0, and optimized MySQL database queries. Set up Docker containers and Kubernetes clusters for scalability, reducing page load times by 25%.",
          },
          {
            year: "June 2019 – April 2020",
            company: "Tech Innovators",
            position: "Junior Full Stack Developer",
            description:
              "Worked on a CRM system using React and Express.js, managing a MongoDB database and integrating APIs like Google Maps. Refactored code to TypeScript and improved frontend performance. Implemented testing with Jest, reducing bugs, and collaborated in code reviews.",
          },
        ],
        education: [
          {
            year: "2022 – 2024",
            institution: "Caraga State University - Main Campus",
            degree: "Master of Information Technology",
          },
          {
            year: "2015 - 2019",
            institution: "Caraga State University - Main Campus",
            degree: "Bachelor of Science in Information Technology",
          },
        ],
        skills: [
          "Frontend Technologies",
          "Backend Technologies",
          "Database Management",
          "Cloud Services",
          "Payment Integration",
          "DevOps Tools",
          "Authentication",
          "Testing Tools",
          "Programming Languages",
        ],
      };
    },
  };
  </script>
  
  <style scoped>
  .left-section {
    background-color: #333;
  }
  .left_section{
    background-color: #c00472;
  }
  
  .left--section{
    color:white;
  }
  
  .right-section {
    background-color: #c00472;
  }
  
  .font-weight-bold {
    font-weight: bold !important;
  }
  
  .grey--text {
    color: #757575 !important;
  }
  
  .profile-picture {
    display: flex; /* Enables flexbox for centering */
    justify-content: center; /* Centers horizontally */
    align-items: center; /* Centers vertically */
    height: 300px; /* Sets height for centering */
  }
  
  .container-margin-top {
    margin-top: 60px;
}
  
  </style>
  
  
