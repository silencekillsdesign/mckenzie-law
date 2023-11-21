<template>
  <v-container>
    <v-form name="contactPage" method="POST" action="/thanks" data-netlify="true" data-netlify-honeypot="bot-field">
      <input type="hidden" name="form-name" value="contactPage">
      <v-container>
        <v-row>
          <input type="hidden" name="form-name" value="contactPage" />
          <v-col
            cols="12"
            md="6">
            <v-text-field
              id="name"
              label="Your Name"
              type="text"
              required></v-text-field>
          </v-col>

          <v-col
            cols="12"
            md="6">
            <v-text-field
              id="email"
              label="E-mail"
              type="email"
              required></v-text-field>
          </v-col>
        </v-row>
        <v-row>
          <v-col>
            <v-textarea id="message" label="Message"></v-textarea>
          </v-col>
        </v-row>
        <v-btn
          class="me-4"
          type="submit">
          submit
        </v-btn>
      </v-container>
    </v-form>
  </v-container>
</template>

