<template>
    <div>
        <v-main class="fill-height pa-0 ma-0">
            <v-container fluid class="mt-0 rounded-lg">
                <v-parallax
                    height="320"
                    src="/img/mountains.jpg">
                    <v-row align="center" justify="center" class="fill-height my-auto rounded-lg">
                        <h1 class="text-white text-h3 text-md-h1 ">DUI Defense</h1>
                    </v-row>
                </v-parallax>
            </v-container>
            <v-container>
                <v-row class="mb-10">
                    <v-col cols="12" offset="0" md="6 offset-1">
                        <h3 class="mb-6">Need DUI Defense in Bozeman?</h3>
                        <p>Montana ranks as the worst state in the nation for drunk driving. The state’s DUI severity score of 84.1 out of 100 is the highest of all states. In 2020, 45% of Montana's road fatalities involved a drunk driver, and there were 473 DUI arrests per 100,000 drivers.</p>
                    </v-col>
                    <v-col cols="12" md="3">
                        <v-img class="circle" src="img/scale.png"></v-img>
                    </v-col>
                </v-row>
                <v-row justify="center" class="bg-blue-accent-3 px-12 py-10 my-10 rounded-lg d-flex align-center justify-center">
                    <v-col md="8" class="text-center">
                        <h3 class="mb-6">minimizing your sentence</h3>
                        <p>Whether you are the subject of a State or Federal investigation, or you have already been arrested and charged, it is crucial to take steps to protect your rights, reputation, and freedom. Without proper legal representation, you may unknowingly waive your rights, which can be used against you in court. Hiring a criminal defense lawyer means having someone who can guide you through the legal process and ensure that your rights are protected at every stage, including interrogations, searches, lineups, and other pre-charge investigation procedures.</p>
                    </v-col>
                </v-row>
                <v-row justify="center" align="center">
                    <v-col cols="10" md="3">
                        <v-img circle class="circle" src="img/wes.jpg"></v-img>
                    </v-col>
                    <v-col cols="12" md="6 offset-1">
                        <h3 class="mb-6">meet wes mckenzie</h3>
                        <p>Wes McKenzie is committed to protecting your rights. We provide zealous and thorough legal representation from the beginning of your case until its conclusion. We will carefully examine the circumstances of your arrest in an effort to determine if your rights were protected. We will carefully explain any potential consequences as we help you make decisions that will ultimately serve your best interests. Wes will not wait until the eve of your court date to discuss the details of your case and leave you guessing as to what the possible outcome will be.</p>
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

<script setup lang="ts">
useSeoMeta({
  title: 'Bozeman DUI Defense - McKenzie Law',
  ogTitle: 'Bozeman DUI Defense - McKenzie Law',
  description: 'Bozeman Defense Attorney Wes McKenzie has a proven track record of beating and minimizing DUI charges.',
  ogDescription: 'Bozeman Defense Attorney Wes McKenzie has a proven track record of beating and minimizing DUI charges.',
})
</script>
