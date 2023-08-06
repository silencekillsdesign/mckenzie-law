<template>
    <v-container>
        <form name="contactPage" action="/thanks" method="POST" netlify>
            <v-container>
                <v-row>
                  <!-- <input type="hidden" name="form-name" value="contactPage" /> -->
                    <v-col
                        cols="12"
                        md="6">
                        <v-text-field
                            v-model="name"
                            label="Your Name"
                            required></v-text-field>
                    </v-col>

                    <v-col
                        cols="12"
                        md="6">
                        <v-text-field
                            v-model="email"
                            label="E-mail"
                            required></v-text-field>
                    </v-col>
                </v-row>
                <v-row>
                    <v-col>
                        <v-textarea label="Message"></v-textarea>
                    </v-col>
                </v-row>
                <v-btn
                    class="me-4"
                    type="submit"
                    >
                    submit
                </v-btn>
            </v-container>
        </form>
    </v-container>
</template>

