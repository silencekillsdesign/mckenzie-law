<template>
    <v-container>
        <form name="contactPage" action="/thanks" method="POST" data-netlify="true">
          <input type="hidden" name="contact-page" value="contactPage" />
            <v-container>
                <v-row>
                  <input type="hidden" name="form-name" value="contactPage" />
                    <v-col
                        cols="12"
                        md="6">
                        <v-text-field
                            v-model="name"
                            :rules="nameRules"
                            :counter="30"
                            label="Your Name"
                            required></v-text-field>
                    </v-col>

                    <v-col
                        cols="12"
                        md="6">
                        <v-text-field
                            v-model="email"
                            :rules="emailRules"
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

<script>
  export default {
    data: () => ({
      valid: false,
      name: '',
      nameRules: [
        value => {
          if (value) return true

          return 'Name is requred.'
        },
        value => {
          if (value?.length <= 40) return true

          return 'Name must be less than 40 characters.'
        },
      ],
      email: '',
      emailRules: [
        value => {
          if (value) return true

          return 'E-mail is requred.'
        },
        value => {
          if (/.+@.+\..+/.test(value)) return true

          return 'E-mail must be valid.'
        },
      ],
    }),
  }
</script>