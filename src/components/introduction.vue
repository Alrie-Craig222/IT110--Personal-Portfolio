<template>
    <a name="home"></a>
    <section class="intro-section mt-n5" id="home">
        <v-row class="align-center px-10">
            <v-col class="pa-6 font-weight-bold py-16">
                <div class="d-flex flex-column justify-center align-center">
                    <span>
                        
                        <div class="d-md-none my-n1 my-n16">
                            <br><br><br><br>
                            <div class="text-h3 ml-n1">I create <br></div>
                            <div class="d-flex flex-row wrapper">
                                <ul class="dynamic-txts">
                                <li><span>with curiosity.</span></li>
                                <li><span>in silence.</span></li>
                                <li><span>from vision to code.</span></li>
                                <li><span>with purpose.</span></li>
                                <li><span>to make ideas real.</span></li>
                                </ul>
                            </div>
                            <v-subheader class=" d-flex text-grey text-center justify-center">
                                Quietly weaving digital solutions into existence.
                            </v-subheader>
                            <div class="d-flex justify-center mt-4">
                                <v-btn :loading="loading[2]" :disabled="loading[2]" @click="load(2)" large elevation="5" color="bblue3"
                                class="text-white mt-1 ml-10 px-10 py-5 text-center d-flex flex-row" href="/resume">Resume</v-btn>
                                <v-btn :loading="loading[2]" :disabled="loading[2]" @click="load(2)" large elevation="5" color="bblue3"
                                class="text-white mt-1 ml-10 px-10 py-5 text-center d-flex flex-row" href="https://github.com/Alrie-Craig222">Portfolio</v-btn>
                            </div>

                            <v-row class="mt-6 d-flex flex-row justify-center">
                                <v-chip class="px-4 ma-3 " color="info" href="https://www.facebook.com/rie.rhie.1" target="blank">
                                    <v-icon left size="20">mdi-facebook</v-icon>
                                    Facebook
                                </v-chip>
                                <v-chip class="px-4 ma-3" color="red" href="YourLinkHere" target="blank">
                                    <v-icon left size="20">mdi-youtube</v-icon>
                                    Youtube
                                </v-chip>
                                <v-chip class="px-4 ma-3" color="orange" href="mailto:alriecraig@gmail.com">
                                    <v-icon left size="20">mdi-email-edit-outline</v-icon>
                                    E-mail
                                </v-chip>
                            </v-row>

                            <v-img src="@/assets/bannerimg.png" width="400px" height="600px" class=" d-md-none ">
                            </v-img>


                        </div>

                        <!-- ----------------------------------------
                            ---------------------------------------- -->
                        <!-- WEB GÖRÜNÜMÜ İÇİN -->

                        <div class="d-none d-md-block">
                            <div class="text-h3 ml-n1">I create <br></div>
                            <div class="d-flex flex-row  wrapper">

                                <ul class="dynamic-txts">
                                    <li><span>with curiosity.</span></li>
                                    <li><span>in silence.</span></li>
                                    <li><span>from vision to code.</span></li>
                                    <li><span>with purpose.</span></li>
                                    <li><span>to make ideas real.</span></li>
                                </ul>
                            </div>
                            <div class="my-2">
                            </div>
                            <v-subheader class="text-grey text-center ">Quietly weaving digital solutions into existence.
                            </v-subheader>

                            <br>
                            <br>
                            <div class="d-flex justify-space-around align-center flex-column flex-md-row">
                                <v-btn :loading="loading[2]" :disabled="loading[2]" @click="load(2)" large elevation="5"
                                    color="#c00472" class="text-white mt-1 ml-10 px-10 py-5 text-center d-flex flex-row"
                                    href="/resume">Resume</v-btn>
                                <v-btn :loading="loading[2]" :disabled="loading[2]" @click="load(2)" large elevation="5"
                                    color="#c00472" class="text-white mt-1 ml-10 px-10 py-5 text-center d-flex flex-row"
                                    href="https://github.com/Alrie-Craig222">Portfolio</v-btn>
                            </div>

                            <v-row class="mt-16 d-flex flex-row justify-center">
                                <v-chip class="px-4 ma-3 " color="info" href="https://www.facebook.com/rie.rhie.1" target="blank">
                                    <v-icon left size="20">mdi-facebook</v-icon>
                                    Facebook
                                </v-chip>
                                <v-chip class="px-4 ma-3" color="red" href="YourLinkHere" target="blank">
                                    <v-icon left size="20">mdi-youtube</v-icon>
                                    Youtube

                                </v-chip>
                                <v-chip class="px-4 ma-3" color="orange" href="mailto:alriecraig@gmail.com">
                                    <v-icon left size="20">mdi-email-edit-outline</v-icon>
                                    E-mail
                                </v-chip>
                            </v-row>
                        </div>
                    </span>
                </div>
            </v-col>
            <v-col class="d-none d-md-block">
                <v-img src="@/assets/bannerimg.png" width="700px" height="500px" class="mx-80 ">
                </v-img>
            </v-col>
        </v-row>
    </section>
    
</template>





<script>
export default {
    name: "SiteIntroduction",
    data() {
        return {
            loading: [],
        }
    },
    methods: {
        load(i) {
            this.loading[i] = true
            setTimeout(() => (this.loading[i] = false), 3500)
        },
    },
}
</script>

<style>
 .text-h3 {
    color: grey;
  }
.custom-loader {
    animation: loader 1s infinite;
    display: flex;
}

@-moz-keyframes loader {
    from {
        transform: rotate(0);
    }

    to {
        transform: rotate(360deg);
    }
}

@-webkit-keyframes loader {
    from {
        transform: rotate(0);
    }

    to {
        transform: rotate(360deg);
    }
}

@-o-keyframes loader {
    from {
        transform: rotate(0);
    }

    to {
        transform: rotate(360deg);
    }
}

@keyframes loader {
    from {
        transform: rotate(0);
    }

    to {
        transform: rotate(360deg);
    }
}


@import url('https://fonts.googleapis.com/css2?family=Poppins:wght@200;300;400;500;600;700&display=swap');



.wrapper {
    display: flex;
}



.wrapper .dynamic-txts {
    margin-left: -5px;
    height: 50px;
    line-height: 50px;
    overflow: hidden;
}

.dynamic-txts li {
    list-style: none;
    color: rgb(143, 141, 141);
    font-size: 30px;
    font-weight: 500;
    position: relative;
    top: 0;
    animation: slide 15s steps(5) infinite;
}

@keyframes slide {
    100% {
        top: -250px;
    }
}

.dynamic-txts li span {
    position: relative;
    margin: 5px 0;
    line-height: 50px;
}

.dynamic-txts li span::after {
    content: "";
    position: absolute;
    left: 0;
    height: 100%;
    width: 100%;
    background: #FAFAFA;
    border-left: 2px solid #90E0EF;
    animation: typing 3s steps(10) infinite;
}

@keyframes typing {

    40%,
    60% {
        left: calc(100% + 10px);
    }

    100% {
        left: 0;
    }
}
</style>

