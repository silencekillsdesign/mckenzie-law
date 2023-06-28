<template>
    <div>
        <v-main class="fill-height pa-0 ma-0">
            <v-container fluid class="mt-0 rounded-lg">
                <v-parallax
                    height="320"
                    src="/img/mountains.jpg">
                    <v-row align="center" justify="center" class="fill-height my-auto rounded-lg">
                        <h1 class="text-white text-h3 text-md-h1 ">Thank You</h1>
                    </v-row>
                </v-parallax>
            </v-container>
            <v-container>
                <v-row class="mb-10">
                    <v-col cols="12" md="6 offset-1">
                        <h3 class="mb-6">Thanks!</h3>
                        <p>Your form has been submitted.</p>
                        <p>Please feel free to give Wes a call any time.</p>
                        <h5><a href="tel:4065774131">406-577-4131</a></h5>
                    </v-col>
                    <v-col cols="12" md="3">
                        <v-img class="circle" src="img/scale.png"></v-img>
                    </v-col>
                </v-row>
        
            </v-container>
        </v-main>
    </div>
</template>

<style lang="scss">
h1 {
    font-family: 'Inter';
    font-weight: 700;
    font-size: 5em;
}

p {
    line-height: 1.8;
}
</style>